# Use gcfntnu/scanpy as base image
FROM gcfntnu/scanpy

# Set the working directory
WORKDIR /workspace

# Install system dependencies
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    openssh-client \
    sshpass \
    && rm -rf /var/lib/apt/lists/*

# Install Python packages
RUN pip install --no-cache-dir \
    jupyter \
    paramiko \
    python-dotenv \
    scp

# Expose port for Jupyter Notebook
EXPOSE 8888

# Copy the current directory contents into the container at /workspace
COPY . /workspace

# Start Jupyter Notebook on container startup
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]