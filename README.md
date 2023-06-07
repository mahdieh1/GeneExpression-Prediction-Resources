# Gene Expression Prediction Resources

This repo accompanies our survey paper:

#### Advancements in Gene Expression Prediction: Methods, Applications, and Future Directions
*Mahdieh Labani, Amin Behehsti, Tracy O’brien, Simon Carlile, Andisheh Partovi*

We list tools, algorithms, data for this area. Feel free to make a pull request for new resources.

---- 

The gene expression prediction model is an AI question. Like any research question, we need to follow three main steps: data preparation, data modelling, and data evaluation. The first step in building a predictive model is to gather all the input data that can be used to inform smarter predictive models. An AI model learns the association between the observed data points and the labels using input features and biological labels from input data. In this case, the input data is the information in the genome. Numerous sequence areas, including genes, promoters, enhancers, and binding sites for regulatory proteins and RNAs, can be found in the genome. However, the main question is which sequence can be beneficial for achieving better performance. Choosing the relevant and adequate input data is critical for providing an efficient and accurate AI model. The survey is organised as follows. 

![alt text](https://github.com/mahdieh1/GeneExpression-Prediction-Resources/blob/main/Figures/Fig1.jpg)

---------------------------------------------------------------------------------------------------------------------------

## Table of Contents

* [Data Preparartion](#Data-Preparartion)
* [Data Modeling](#Data-Modeling)
    - [First group: Genomic Sequence](#First-group--Genomic-Sequence)
    - [Second group: Histone marks](#Second-group--Histone-marks)
    - [Third group: Transcription factor binding sites](#Third-group--Transcription-factor-binding-sites)
    - [Fourth group: DNase I hypersensitive measurements](#Fourth-group--DNase-I-hypersensitive-measurements)
    - [Fifth group: Massively Parallel Reporter Assay (MPRAs)](#Fifth-group--Massively-Parallel-Reporter-Assay-(MPRAs))
* [Data Modeling](#Data-Modeling)
* [Author Info](#author-info)
* [Acknowledgements](#Acknowledgements)
     
------------------------------------------------------------------------------------------------------------------------
## Data Preparartion

Gene expression is a highly regulated process that involves the conversion of genetic information stored in DNA into functional gene products, such as proteins or RNA molecules. The complex interplay of various factors influences gene expression, and understanding these dynamics is crucial for understanding the underlying mechanisms. Gene expression prediction models categorised into five groups based on these input factors including genomic sequence, histone marks, transcription factors, DNase I hypersensitivity measurements, and MPRA.

![alt text](https://github.com/mahdieh1/GeneExpression-Prediction-Resources/blob/main/Figures/Figure2-new.jpg)

### First group: Genomic Sequence 

| Method | Year | Availability of code | 	AI/ML models | Upstream | Downstream | Performance measure |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
| Kelley, D.R., et al., Sequential regulatory activity prediction across chromosomes with convolutional neural networks. Genome research, 2018. 28(5): p. 739-750.| 2018 |	https://github.com/calico/basenji | CNN & dilated layers	| 65.5kbp |	65.5kbp |	PCC = 0.85 |
| Kelley, D.R., Cross-species regulatory sequence activity prediction. PLoS computational biology, 2020. 16(7): p. e1008050. | 2020 |	https://github.com/calico/basenji | CNN |	131,072bp |	 | PCC = 0.632 |
| Agarwal, V. and J. Shendure, Predicting mRNA Abundance Directly from Genomic Sequence Using Deep Convolutional Neural Networks. Cell Rep, 2020. 31(7): p. 107663. | 2020 |	https://github.com/vagarwal87/Xpresso | CNN |	7kbp	| 3.5kbp |	R2 = 0.59 |
| Avsec, Ž., et al., Effective gene expression prediction from sequence by integrating long-range interactions. Nature methods, 2021. 18(10): p. 1196-1203. | 2021 |	https://github.com/deepmind/deepmind-research/tree/master/enformer | Transformer model |	100bp	| 100bp |	PCC = 0.85 |
| Zhang, Y., X. Zhou, and X. Cai, Predicting gene expression from DNA sequence using residual neural network. bioRxiv, 2020: p. 2020.06. 21.163956. | 2022	| -	| Resnet |	70bp |	25bp |	PCC = 0.8026 |
| Zeng, W., Y. Wang, and R. Jiang, Integrating distal and proximal information to predict gene expression via a densely connected convolutional neural network. Bioinformatics, 2020. 36(2): p. 496-503. | 2019	| https://github.com/wanwenzeng/DeepExpression | CNN |	1000bp |	1000bp	| PCC= 0.8 |
| Karbalayghareh, A., M. Sahin, and C.S. Leslie, Chromatin interaction–aware gene regulatory modeling with graph attention networks. Genome Research, 2022. 32(5): p. 930-944. | 2022 |	https://github.com/karbalayghareh/GraphReg |	GAT & CNN |	6Mb |	| PCC = 0.835 |
| Bigness, J., et al., Integrating Long-Range Regulatory Interactions to Predict Gene Expression Using Graph Convolutional Networks. J Comput Biol, 2022. 29(5): p. 409-424. | 2022 |	https://github.com/rsinghlab/GC-MERGE | GCN |	- |	-	|AUROC = 0.92 |
| Pipoli, V., et al., Predicting gene expression levels from DNA sequences and post-transcriptional information with transformers. Computer Methods and Programs in Biomedicine, 2022. 225: p. 107035. | 2022 | https://github.com/geneexpressionpolito/Predicting-gene-expression-levels-from-DNA-sequences-and-post-transcriptional-info-with-transformers | Transformer model & DeepLncLoc	| 10kbp	| - |	R2 = 0.764 |


### Second group: Histone marks 

| Method | Year | Availability of code | 	AI/ML models | Upstream | Downstream | Performance measure |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
| Karlić, R., et al., Histone modification levels are predictive for gene expression. Proceedings of the National Academy of Sciences, 2010. 107(7): p. 2926-2931. | 2010 |	-	| LR |	4,001bp |	 | R2 = 0.77 |
| Costa, I.G., et al., Predicting gene expression in T cell differentiation from histone modifications and transcription factor binding affinities by linear mixture models. BMC bioinformatics, 2011. 12(1): p. 1-10. | 2011	| - |	LR |	8kbp |	2kbp |	MSE = 0.25 |
| Cheng, C. and M. Gerstein, Modeling the relative relationship of transcription factor binding and histone modifications to gene expression levels in mouse embryonic stem cells. Nucleic acids research, 2012. 40(2): p. 553-568. | 2012 |	- |	SVM |	4kbp |	4kbp |	R2=0.50 |
| Dong, X., et al., Modeling gene expression using chromatin features in various cellular contexts. Genome biology, 2012. 13(9): p. 1-17. | 2012 |	-	| RF |	2kbp |	2kbp |	PCC = 0.71 |
| Ho, B.H., R.M.K. Hassen, and N.T. Le. Combinatorial roles of dna methylation and histone modifications on gene expression. in Some Current Advanced Researches on Information and Computer Science in Vietnam: Post-proceedings of The First NAFOSTED Conference on Information and Computer Science. 2015. Springer. | 2015 |	-	| CN2-SD |	1kbp |	1kbp |	F-score = 2.794 |
| Li, J., et al. Using epigenomics data to predict gene expression in lung cancer. in BMC bioinformatics. 2015. BioMed Central. | 2015 |	https://github.com/lanagarmire/epiPredictor | ReliefF	| 1500bp	| 200bp	| AUC = 0.836 |
| Singh, R., et al., DeepChrome: deep-learning for predicting gene expression from histone modifications. Bioinformatics, 2016. 32(17): p. i639-i648. | 2016	| https://github.com/QData/DeepChrome | CNN |	5kbp |	5kbp |	AUC = 0.80 |
| Singh, R., et al., Attend and predict: Understanding gene regulation by selective attention on chromatin. Advances in neural information processing systems, 2017. 30. | 2017	| https://github.com/QData/AttentiveChrome | LSTM	| 5kbp |	5kbp |	F1 score = 0.56 |
| Sekhon, A., R. Singh, and Y. Qi, DeepDiff: DEEP-learning for predicting DIFFerential gene expression from histone modifications. Bioinformatics, 2018. 34(17): p. i891-i900. | 2018 |	https://github.com/QData/DeepDiffChrome | LSTM |	5kbp |	5kbp |	F1 score = 0.6 |

### Third group: Transcription factor binding sites 
| Method | Year | Availability of code | 	AI/ML models | Upstream | Downstream | Performance measure |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | 

TFAS[46]
2009	-	PCA	500 bps for E2f1 and 5,000 bps for other TFs	R2 = 0.650
TEPIC[45]
2017	www.github.de/schulzlab/TEPIC
Elastic net regression
	3kbp and 5Kbp	Mean test correlation = 0.68

### Fourth group: DNase I hypersensitive measurements 
### Fifth group: Massively Parallel Reporter Assay (MPRAs) 


