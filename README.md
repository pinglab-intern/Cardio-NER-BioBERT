# CVD-NER-BioBERT
Named Entity Recognition with BioBERT in CVD documents. This project conducts the Named Entity Recognization (74 biomedical entities from anatomy, physiology, omics (genome, proteome, transcriptome, metabolom, microbiome), drugs and chemicals. We will start from pretrained BioBert to fintune it for NER model with BioNLP data. The fine tuined model will assist to identify biomedical entites in CVD documents.

### Data Sources:
 - PubMed Documents (CVD)
 - MeSH Descriptors (CVD)
 - BioNLP (Sentence and Tags)

### Pretrained Model
-  BioBERT (Pubmed -v1.1 from HuggingFace)

### Fine Tuning
- Fine tuning with BioNLP data will be conducted

### Application
The recognized named entities will be used to create a knowledgegraph for CVD documents. It will help to conduct
-  (1) smart queries for data exploration, create data summary, visualization and analysis 
-  (2) create graph embedding and conduct dimentionality reduction and visualization (PCA, t-SNE)
-  (3) Graph Neural Network specially link Prediction between CVD diseases and molecular mechanism (gene,  proteins, pathways)


