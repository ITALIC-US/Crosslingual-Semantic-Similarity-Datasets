# Crosslingual Semantic Similarity Datasets

## Description
This dataset for the cross-lingual semantic similarity task (Spanish-English) is formed by different corpora that have been transformed. Below you will find the specific process applied to each one and the original source, but before that, we will explain the content format they all share.

## Format
Each corpus included in this dataset contains two types of files:
* '*.4c': Each line contains 4 sentences separated by a tab (\t). The first 2 are the Spanish and English sentences to be compared, while the last 2 are the machine translation version of the first 2. The resulting format is: 's1(Spanish) s2(English) s3(English MT version of s1) s4(Spanish MT version of s2). 
* '*.gs': Gold standard. Shows the similarity measure for each row of the corresponding '4c' file.

## Data

* SE-12-TE: Adapted version of the 'Cross-lingual textual entailment' (CLTE-SemEval) task of SemEval 2012 (see IMPORTANT NOTE at the end of this file). The original tags associated with each pair of sentences (directionality of the entailment) has been mapped to a similarity score. Duplicate sentences have been discarded so that each sentence only appears once in the file. 

## IMPORTANT NOTE

* The original CLTE-SemEval dataset is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.
Publications or presentations containing results obtained through the use of CLTE-SemEval should cite the following reference:
    * Matteo Negri, Luisa Bentivogli, Yashar Mehdad, Danilo Giampiccolo, and Alessandro Marchetti. 2011.
    Divide and Conquer: Crowdsourcing the Creation of Cross-Lingual Textual Entailment Corpora.
    Proceedings of the 2011 Conference on Empirical Methods in Natural Language Processing (EMNLP 2011).
 
* SE-14-STS: Adapted version of the 'Semantic Textual Similarity' (mono-lingual) task of SemEval 2014. The second sentence of each original pair has been manually translated to English.  

* SE-15-STS: Adapted version of the 'Semantic Textual Similarity' (mono-lingual) task of SemEval 2015. The second sentence of each original pair has been manually translated to English.  

* SE-16-STS-news & SE-16-STS-multi: Original data from the 'Cross-lingual Semantic Textual Similarity' task of SemEval 2016, considering the 'multisource' and 'news' files. The only change made has been the concatenation of the translated versions (MT) of the original pairs of sentences.

## Citations
If you use material from this dataset, please cite the following references:

* Fernando Enríquez, Fermín Cruz, F. Javier Ortega, José A. Troyano (2017)
  Similitud español-inglés a través de word embeddings
  Procesamiento del Lenguaje Natural, 59.

* Matteo Negri, Luisa Bentivogli, Yashar Mehdad, Danilo Giampiccolo, and Alessandro Marchetti. 2011.
  Divide and Conquer: Crowdsourcing the Creation of Cross-Lingual Textual Entailment Corpora.
  Proceedings of the 2011 Conference on Empirical Methods in Natural Language Processing (EMNLP 2011).
