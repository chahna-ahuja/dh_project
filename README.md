<h1 id="notebook-title" data-toc="false">
ALL THE METADATA'S A STAGE NOTEBOOK 
</h1>
<h2 id="notebook-subtitle" data-toc="false">
Exploratory Bibliographic and Text Network Analysis of British Comedy Dramas Across 17th-19th Centuries
</h2>
<h3 id="author" data-toc="false">
Author: Chahna Ahuja
</h3>
<h3 id="course" data-toc="false">
Course: Introduction to Digital Humanities CLass (2025-26) Dr. Margherita Fantoli at KU Leuven (Msc Digital Humanities)
</h3>
---
<h1 id="introduction" data-toc="false">
Introduction to the Project
</h1>

This project explores the **British Library’s bibliographic dataset of digitized British dramas from the 17th–19th centuries**, using an **exploratory distant reading** approach.  

The workflow of this notebook proceeds in three stages:  

1. **Descriptive Statistics and Visualization of the Dataset**  
   Provides a structured overview of the dataset for both the researcher and the reader, helping understand dataset size, structure and suitability for further analysis.  

2. **Exploratory Data Analysis on Comedy Subdataset**  
   Investigateso examine temporal trends in publications, spatial networks of publishing locations, authorship distribution, and lexical patterns of comedy titles.

3. **Text Mining and Network Analysis**  
   Constructs a **syntactic dependency network** of frequent lemmas in comedy titles to address the central research question:  

   > **How do 17th–19th century British comedy titles encode gendered roles and archetypes, and what do they reveal about the social expectations of the period?**
---
<h2 id="dataset" data-toc="false">
Github Repository Structure
</h2>

- [README.md](https://github.com/chahna-ahuja/dh_project/blob/main/README.md)

- **data/**
  - [dh_group7_drama.csv](https://github.com/chahna-ahuja/dh_project/blob/main/data/dh_group7_drama.csv)
  - [final_drama_comedy.csv](https://github.com/chahna-ahuja/dh_project/blob/main/data/final_drama_comedy.csv)
  - [final_drama_tragedy.csv](https://github.com/chahna-ahuja/dh_project/blob/main/data/final_drama_tragedy.csv)
  - [final_drama_play.csv](https://github.com/chahna-ahuja/dh_project/blob/main/data/final_drama_play.csv)
  - [raw/](https://github.com/chahna-ahuja/dh_project/tree/main/data/raw)

- **data_analysis/**
  - [chahna_dataproject_script.ipynb](https://github.com/chahna-ahuja/dh_project/blob/main/data_analysis/chahna_dataproject_script.ipynb)
  - [chahna_dataproject_jupyternotebook.html](https://github.com/chahna-ahuja/dh_project/blob/main/data_analysis/chahna_dataproject_jupyternotebook.html)

- **network_analysis/**
  - [comedy_network_nodes.csv](https://github.com/chahna-ahuja/dh_project/blob/main/network_analysis/network_nodes.csv)
  - [comedy_network_edges.csv](https://github.com/chahna-ahuja/dh_project/blob/main/network_analysis/network_edges.csv)
  - [toplemmas_network.png](https://github.com/chahna-ahuja/dh_project/blob/main/network_analysis/toplemmas_network.png)
  - [chahna_dataproject_network.gephi](https://github.com/chahna-ahuja/dh_project/blob/main/network_analysis/chahna_dataproject_network.gephi)

- **data_visualization/** #charts and data visualizations from python

- **project_management/** #project management plant + gantt chart

- **visual_assets/** #visual aesthetic images for python html


---
<h2 id="dataset" data-toc="false">
Dataset
</h2>

- **Original Source:** British Library digitized drama metadata, cleaned as part of a **group assignment** for **Introduction to Digital Humanities CLass, taught by Dr. Margherita Fantoli, in academic year 2025-26 at KU Leuven (Msc Digital Humanities)**.
- **Data Wrangling Process:**  
  - **OpenRefine** used to wrangle data while preserving original information.  
  - **Facet filtering** to isolate subsets and identify inconsistencies.  
  - **GREL scripting** to standardize and transform columns.  
  - **WikiData reconciliation** to enrich author information with contextual metadata.  
- **Cleaned Datasets:** Main dataset: dh_group7_drama.csv. Three subdatasets: *Comedy*, *Tragedy*, *Plays* cleaned in *OpenRefine* by Chahna Ahuja, Xinran Liu and Liangyu Gan, respectively as a group project component for this assignment. ([check this Github repository to know more!](https://github.com/chahna-ahuja/dh-g7-project)
---
<h2 id="methods" data-toc="false">
Methods
</h2>

- **Data Analysis Environment**: Jupyter Notebook combining code, output, and narrative. Interactive charts via Plotly, word clouds via WordCloud. Use of Wikidata API.
- **Text Mining Using NLP**: spaCy (tokenization, lemmatization, dependency parsing), NLTK (preprocessing & exploratory analysis)
- **Network Visualization**: Gephi used to construct the comedy title syntactic dependency network to explore the hypothesis.
---
<h2 id="methods" data-toc="false">
Tools for Python and Gephi 
</h2>

- For reproducing the python notebook, first **pip install** the packages in [requirements.txt](https://github.com/chahna-ahuja/dh_project/blob/main/requirements.txt)
-  Go to [https://gephi.org/users/download/](https://gephi.org/users/download/) and download Gephi. Open Gephi, and import nodes and edges CSV files from [here](https://github.com/chahna-ahuja/dh_project/tree/main/network_analysis) 
- To view HTML notebook without downloading it, go [here](https://nbviewer.org/github/chahna-ahuja/dh_project/blob/main/data_analysis/chahna_dataproject_script.ipynb)
