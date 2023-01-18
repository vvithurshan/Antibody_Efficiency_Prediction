# Antibody Efficiency Prediction with Amino Acid sequence.
# Description

## Input Format
The concatenated amino acid sequence of CDR of the antibody and epitope of the Antigen
### Eg
Amino acid sequence of CDR of Antibody = ALALHFYPGVYDDYGPPIARGVN          
Amino acid sequecne of epitope of the Antigen = TLDSWK         
Valid input = ALALHFYPGVYDDYGPPIARGVNTLDSWK

## Table
| Method      | Accuracy |
| --------- | -----|
|**Logistic Regression**  | - |
|- One hot Encoding | 86.37 %|
|- Blosum | 86.92 % |
|- NLF | 86.92 % |
| **SVM** (kernal = linear)   |   - |
|- One hot Encoding | 86.10 %|
|- Blosum | 87.19 % |
|- NLF | 86.10 %|
| **ProtBert**      |    - |
| -prot_bert tokenizer| 84.42 %
| **ProtBert_bfd** |     -  |
|-Prot_bert_bfd tokenizer| 83.60 %
| **ProtCNN** | -|
|- One hot Encoding|88 %|
|- Blosum |87 %|
|- NLP| 87 %|
|- BeplerEmbedder| 87 %|
|- CPCProtEmbedder |76 %|
|- FastTextEmbedder | 64 %|
|- GloveEmbedder | 64 %|
|- PLUSRNNEmbedder | 64 %|
| - ProtTransBertBFDEmbedder| 83 %|
| - Word2VecEmbedder| 64 %|


## References
- https://github.com/agemagician/ProtTrans/blob/master/Fine-Tuning/ProtBert_BFD_FineTuning_MS.ipynb
- https://huggingface.co/Rostlab/prot_bert_bfd
- https://huggingface.co/Rostlab/prot_bert
- https://towardsdatascience.com/protein-sequence-classification-99c80d0ad2df
- https://dmnfarrell.github.io/bioinformatics/mhclearning
