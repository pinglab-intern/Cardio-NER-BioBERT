# CVD-NER-BioBERT

#### Title: Named Entity Recognition with BioBERT in CVD documents. 

#### Task: To conducts the Named Entity Recognization (74 biomedical entities: anatomy, biomolecules, chemicals) from Cardiovascular Disease (CVD) documents from PubMed

We will start from pretrained BioBert to fintune it for NER model with BioNLP data. The fine tuined model will assist to identify biomedical entites in CVD documents.

### Data Sources:
 - [PubMed Documents](https://pubmed.ncbi.nlm.nih.gov/download/) (CVD)
 - [MeSH Descriptors](https://meshb.nlm.nih.gov/treeView) (CVD)
 - [BioNLP](https://www.ncbi.nlm.nih.gov/research/bionlp/Data/) (Sentence and Tags)

### Pretrained Model
-  [BioBERT](https://github.com/dmis-lab/biobert) a pre-trained biomedical language representation model for biomedical text mining from DMIS-Lab.

### BioNLP Tags:


1. I-Cellular_component
2. E-Gene_or_gene_product
3. I-Organism_subdivision
4. I-Organism_substance
5. B-Gene_or_gene_product
6. B-Cancer
7. I-Cancer
8. E-Pathological_formation
9. I-Pathological_formation
10. S-Organism_substance
11. S-Organ
12. E-Organ
13. I-Immaterial_anatomical_entity
14. E-Cell
15. I-Simple_chemical
16. E-Tissue
17. B-Organism
18. S-Cellular_component
19. S-Pathological_formation
20. I-Amino_acid
21. E-Anatomical_system
22. S-Developing_anatomical_structure
23. B-Immaterial_anatomical_entity
24. B-Protein
25. I-Chemical
26. S-Organism
27. I-Gene_or_gene_product
28. I-Cell
29. E-Multi-tissue_structure
30. B-Organism_subdivision
31. E-Cellular_component
32. S-Chemical
33. S-Protein
34. B-Simple_chemical
35. E-Organism
36. B-Developing_anatomical_structure
37. S-Multi-tissue_structure
38. S-Immaterial_anatomical_entity
39. B-Organism_substance
40. E-Organism_substance
41. E-Simple_chemical
42. I-Tissue
43. E-Immaterial_anatomical_entity
44. I-Organism
45. I-Protein
46. S-Organism_subdivision
47. E-Cancer
48. I-Developing_anatomical_structure
49. S-Tissue
50. E-Chemical
51. S-Amino_acid
52. O
53. S-Gene_or_gene_product
54. E-Organism_subdivision
55. B-Anatomical_system
56. B-Chemical
57. B-Cell
58. E-Developing_anatomical_structure
59. I-Multi-tissue_structure
60. B-Pathological_formation
61. B-Cellular_component
62. B-Organ
63. I-Anatomical_system
64. S-Cell
65. E-Amino_acid
66. B-Tissue
67. S-Simple_chemical
68. E-Protein
69. B-Multi-tissue_structure
70. I-Organ
71. S-Cancer
72. B-Amino_acid
73. S-Anatomical_system
74. PAD


### Fine Tuning
- Fine tuning with BioNLP data will be conducted with BioNLP data to identify 74 biomedical entities from CVD documents.

### Application
The recognized named entities will be used to create a knowledgegraph for CVD documents. It will help to conduct
-  (1) smart queries for data exploration, create data summary, visualization and analysis 
-  (2) create graph embedding and conduct dimentionality reduction and visualization (PCA, t-SNE)
-  (3) Graph Neural Network specially link Prediction between CVD diseases and molecular mechanism (gene,  proteins, pathways)


### References
1. [BioBERT: a pre-trained biomedical language representation model for biomedical text mining](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7703786/)
