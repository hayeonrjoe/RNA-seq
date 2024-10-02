<h1>🧬 RNA-seq</h1>
RNA sequencing analysis practice<br/><br/>

<h2>🧫 RNA-seq Experiments</h2>
<ol>
  <li>Healthy Mouse Liver scRNA-seq</li>
  <details>
  <summary>Summary</summary>
    <p>
      Utilizing Python 3.11.9 and code adapted from the "Preprocessing and clustering 3k PBMCs (legacy workflow)" tutorial, I analyzed scRNA-seq data from healthy mouse liver tissue obtained from GEO Sample GSM4041174, which was stored on a server. After preprocessing, including QC and normalization, I performed PCA and clustering using the Leiden algorithm. Marker genes for each cluster were identified using statistical tests, and descriptive names were assigned based on information from the "Mouse Genome Informatics" database. Subsequently, appropriate group or cluster names were assigned based on the genes in each group. The analysis was conducted in a Jupyter Notebook within Visual Studio Code, and the data originated from 10X Genomics Single cell 3' gene expression V2 sequencing on an Illumina HiSeq 4000 instrument.
    </p>
  </details>
    <li>Healthy Human Liver scRNA-seq</li>
  <details>
  <summary>Summary</summary>
    <p>
      The scRNA-seq analysis of healthy human liver tissue (GEO Sample GSM7802682) was conducted within a Docker environment using the gcfntnu/scanpy image from Docker Hub, configured with volume mounts and port mappings through docker-compose. Data retrieval involved SSH and SCP protocols to transfer files to a local directory (/workspace/data). The analysis identified distinct clusters in the PCA plot, highlighting varying CST3 expression levels that may correlate with different biological states or cell types. Key genes like SLCO2A1 and DNAJC11 associated with principal components PC1 and PC2 demonstrated significant loading values, suggesting their pivotal role in driving these variations. Additionally, a notable proportion of mitochondrial gene counts was observed, potentially indicating poorer data quality in the analyzed dataset.
    </p>
  </details>
</ol>
