#### Title: 

***Building Named Entity Recognition model with fine tuning BioBERT - a data engineering approach***

#### Detail: 

This project is about data engineering of Cardiovascular documents where we transform the data from raw text to mapping of named entities through transfer learning [1][2]. The mapping of documents to entities can be implemented for designing Knowledgegraph and machine learning models. To conducts the Named Entity Recognization (74 biomedical entities: anatomy, biomolecules, chemicals) from Cardiovascular Disease (CVD) documents from PubMed, we propose to build NER model with pretrained bioBERT model in NLP. 

In brief, we will start from pretrained BioBert to fintune it for NER model with BioNLP data. The fine tuined model will assist to identify biomedical entites in CVD documents.

### Data Sources:
 - [PubMed Documents](https://pubmed.ncbi.nlm.nih.gov/download/) (CVD)
 - [MeSH Descriptors](https://meshb.nlm.nih.gov/treeView) (CVD)
 - [BioNLP](https://www.ncbi.nlm.nih.gov/research/bionlp/Data/) (Sentence and Tags)

### Pretrained Model
-  [BioBERT](https://github.com/dmis-lab/biobert) a pre-trained biomedical language representation model for biomedical text mining from DMIS-Lab.

### BioNLP Tags:

```
1. I-Cellular_component  2. E-Gene_or_gene_product  3. I-Organism_subdivision
4. I-Organism_substance  5. B-Gene_or_gene_product  6. B-Cancer
7. I-Cancer   8. E-Pathological_formation   9. I-Pathological_formation
10. S-Organism_substance  11. S-Organ  12. E-Organ
13. I-Immaterial_anatomical_entity  14. E-Cell  15. I-Simple_chemical
16. E-Tissue  17. B-Organism  18. S-Cellular_component
19. S-Pathological_formation  20. I-Amino_acid  21. E-Anatomical_system
22. S-Developing_anatomical_structure 23. B-Immaterial_anatomical_entity
24. B-Protein  25. I-Chemical  26. S-Organism  27. I-Gene_or_gene_product
28. I-Cell  29. E-Multi-tissue_structure  30. B-Organism_subdivision
31. E-Cellular_component  32. S-Chemical  33. S-Protein
34. B-Simple_chemical  35. E-Organism  36. B-Developing_anatomical_structure
37. S-Multi-tissue_structure  38. S-Immaterial_anatomical_entity
39. B-Organism_substance  40. E-Organism_substance  41. E-Simple_chemical
42. I-Tissue  43. E-Immaterial_anatomical_entity  44. I-Organism
45. I-Protein  46. S-Organism_subdivision  47. E-Cancer
48. I-Developing_anatomical_structure  49. S-Tissue
50. E-Chemical  51. S-Amino_acid  52. O
53. S-Gene_or_gene_product 54. E-Organism_subdivision
55. B-Anatomical_system  56. B-Chemical  57. B-Cell  
58. E-Developing_anatomical_structure  59. I-Multi-tissue_structure  
60. B-Pathological_formation  61. B-Cellular_component  62. B-Organ
63. I-Anatomical_system 64. S-Cell  65. E-Amino_acid
66. B-Tissue 67. S-Simple_chemical 68. E-Protein
69. B-Multi-tissue_structure 70. I-Organ 71. S-Cancer
72. B-Amino_acid 73. S-Anatomical_system 74. PAD

```

### Fine Tuning
- Fine tuning with BioNLP data will be conducted with BioNLP data to identify 74 biomedical entities from CVD documents.

### Project Walkthrough:
1. Learn more about Transformer (e.g., embedding and positional encoding, multihead self attention, layer addition and normalization)
2. Learn more about BERT (e.g., model architecture, building pretrained model)
3. Learn more about building bioBERT with pubmed documents as data sources
4. Explore advanced NLP libraries (Huggingface, simpletransformer) with tutorials
5. Preparing BioNLP data with sentences and tags for fine tuning bioBERT model.
6. Train NER model with the pretrained bioBERT model with sentences and tags obtaind from BioNLP.
7. Prepare Cardiovascular documents for implementing NER model for document to entities mapping.
8. Prepare the document to entities mapping.

### Application
The recognized named entities will be used to create a knowledgegraph for CVD documents. It will help to conduct

-  (1) smart queries for data exploration, create data summary, visualization and analysis 
-  (2) create graph embedding and conduct dimentionality reduction and visualization (PCA, t-SNE)
-  (3) Graph Neural Network specially link Prediction between CVD diseases and molecular mechanism (gene,  proteins, pathways)


### Educational Goal:

This project offers an ooprtunity to get familiar with advanced NLP models (e.g., transformer and BioBERT) and implementation of Named entity recognition over CVD documents. 

### Scientific Goal:

This project offers a new data engineeering concept which could deliver high quality data to assist other scientific exploration (e.g. knowledge graph, graph neural network, entity resolution, concept normalization)

### References
1. [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7703786/)
2. [Tagging Genes and Proteins with BioBERT](https://towardsdatascience.com/tagging-genes-and-proteins-with-biobert-c7b04fc6eb4f)
