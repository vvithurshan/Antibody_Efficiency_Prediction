# Antibody_Efficiency_Prediction

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
| **Prot bert**      |    84.42 % |
| **prot_bert_bfd** |     83.60 %  |

## Conclusion
Based on the results, it seems SVM with BLOSUM encoding method outperfomed other methods.


## References
- https://github.com/agemagician/ProtTrans/blob/master/Fine-Tuning/ProtBert_BFD_FineTuning_MS.ipynb
- https://huggingface.co/Rostlab/prot_bert_bfd
- https://huggingface.co/Rostlab/prot_bert
- https://towardsdatascience.com/protein-sequence-classification-99c80d0ad2df
- https://dmnfarrell.github.io/bioinformatics/mhclearning
