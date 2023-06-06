# GeneExpression-Prediction-Resources

This repo accompanies our survey paper:

Advancements in Gene Expression Prediction: Methods, Applications, and Future Directions

We list tools, algorithms, data for this area. Feel free to make a pull request for new resources.
---- 

The gene expression prediction model is an AI question. Like any research question, we need to follow three main steps: data preparation, data modelling, and data evaluation. The first step in building a predictive model is to gather all the input data that can be used to inform smarter predictive models. An AI model learns the association between the observed data points and the labels using input features and biological labels from input data. In this case, the input data is the information in the genome. Numerous sequence areas, including genes, promoters, enhancers, and binding sites for regulatory proteins and RNAs, can be found in the genome. However, the main question is which sequence can be beneficial for achieving better performance. Choosing the relevant and adequate input data is critical for providing an efficient and accurate AI model. The survey is organised as follows. 

![alt text](https://github.com/mahdieh1/GeneExpression-Prediction-Resources/blob/main/Figures/Fig1.jpg)

# Table of Contents

- [Gene expression prediction](#Gene-expression-prediction)

  * [Data Preparartion](#Data-Preparartio)
  * [Data Modeling](#Data-Modeling)
  * [Model Evaluation](#Model-Evaluation)
    

## Data Preparartion
Gene expression is a highly regulated process that involves the conversion of genetic information stored in DNA into functional gene products, such as proteins or RNA molecules. The complex interplay of various factors influences gene expression, and understanding these dynamics is crucial for understanding the underlying mechanisms. Gene expression prediction models categorised into five groups based on these input factors including genomic sequence, histone marks, transcription factors, DNase I hypersensitivity measurements, and MPRA.

![alt text](https://github.com/mahdieh1/GeneExpression-Prediction-Resources/blob/main/Figures/Figure2-new.jpg)

### Theme 1: Facilitating Understanding of Human Biology

![human_bio](figs/fig5.png)


#### Task 1: DNA-protein and RNA-protein binding prediction

**Task Description** Given a set of DNA/RNA sequences predict their binding scores. After training,use feature importance attribution methods to identify the motifs. 


[Jian Zhou and Olga G Troyanskaya. Predicting effects of noncoding variants with deep learning–based
sequence model. Nature Methods, 12(10):931–934, 2015.](https://pubmed.ncbi.nlm.nih.gov/26301843/)
