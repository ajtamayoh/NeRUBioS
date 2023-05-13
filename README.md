# NeRUBioS dataset and source code for the paper "Augmenting a Spanish Clinical Dataset for Transformer-Based Linking of Negations and their Out-of-Scope References" 

Authors:

Antonio Tamayo (ajtamayo2019@ipn.cic.mx, ajtamayoh@gmail.com)

Diego A. Burgos (burgosda@wfu.edu)

Alexander Gelbulkh (gelbukh@gelbukh.com)

For bugs or questions related to the code, do not hesitate to contact us (Antonio Tamayo: ajtamayoh@gmail.com)

If you use this code please cite our work:

Comming soon...

## Abstract

A negated statement is a semantic unit made up of three components, namely, the negation cue, the negation scope, and the negation reference, which may or may not be within the negation scope. While many have researched on the negation cue and scope, little to no attention has been paid to identifying negation references located out of the negation scope notwithstanding they account for almost half of negations. In this work, we aim at identifying out-of-scope references (OSRs) to restore the sense of truncated negated statements extracted by negation detection systems. For this, we add OSRs annotations to augment the largest available Spanish clinical dataset. We also fine-tune three strong BERT-based models and address negation detection, uncertainty detection, and OSR identification and linking with its respective negation scope using transfer learning. Our best model keeps state-of-the-art performance at negation detection and, at the same time, sets a competitive baseline for OSR identification (Macro F1= 0.56) and linking (Macro F1= 0.86). We back up these findings with relevant statistics from the newly annotated data set as well as from a thorough literature survey.

### How to use our model

[Hugging Face Model](https://huggingface.co/ajtamayoh/NeRUBioS_RoBERTa_Training_Testing/settings)

### How to replicate our experiments

[source code](https://github.com/ajtamayoh/NeRUBioS/blob/main/Source%20code.ipynb)
