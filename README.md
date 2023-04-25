# Antibody Efficiency Prediction with Amino Acid sequence.
# Description
It used different methods such as logistic regression, SVM, ProtBert and ProtCNN with various encodings and embeddings. It also provides a table of accuracy scores for each method. <br >

## Input Format
The concatenated amino acid sequence of CDR of the antibody and epitope of the Antigen
### Eg
Amino acid sequence of CDR of Antibody = ALALHFYPGVYDDYGPPIARGVN          
Amino acid sequecne of epitope of the Antigen = TLDSWK         
Valid input = ALALHFYPGVYDDYGPPIARGVNTLDSWK

The concatenated amino acid sequence of CDR of the antibody and epitope of the antigen refers to the combination of the amino acid sequences of the complementarity-determining regions (CDRs) of the antibody and the epitope of the antigen they bind to. <br />

The CDRs are the most variable regions of an antibody, and they are responsible for the specificity of the antibody-antigen interaction. The epitope is the specific part of the antigen that the antibody recognizes and binds to. <br />

To create the concatenated amino acid sequence, you need to take the amino acid sequence of the CDR of the antibody and append it to the amino acid sequence of the epitope of the antigen. The resulting sequence should be a single string of amino acid residues with no spaces or separators between them. <br />

For example, if the amino acid sequence of the CDR of the antibody is "ALALHFYPGVYDDYGPPIARGVN" and the amino acid sequence of the epitope of the antigen is "TLDSWK", then the valid concatenated amino acid sequence would be "ALALHFYPGVYDDYGPPIARGVNTLDSWK". <br />

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
