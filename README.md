# Augmenting a Spanish Clinical Dataset for Transformer-Based Linking of Negations and their Out-of-Scope References

### NeRUBioS dataset and full source code 

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

[Hugging Face Model](https://huggingface.co/ajtamayoh/NeRUBioS_RoBERTa_Training_Testing)

### How to replicate our experiments

[source code](https://github.com/ajtamayoh/NeRUBioS/blob/main/Source%20code.ipynb)

### NeRUBioS statistics

| Features                                | Training | Development | Testing | Overall  |
| --------------------------------------- | -------- | ----------- | ------- | -------- |
| Number of sentences                     | 13,832   | 1,840       | 2,765   | 18,437   |
| Number of tokens                        | 256,083  | 35,436      | 51,269  | 342,788  |
| Number of types                         | 18,606   | 6,297       | 7,659   | 32,562   |
| Number of sentences with OSRs           | 2,660    | 380         | 566     | 3,606    |
| Number of multiword OSRs                | 1,912    | 298         | 426     | 2,636    |
| Number of discontinuous OSRs            | 238      | 46          | 52      | 336      |
| Number of sentences with multiple OSRs  | 158 (1.2%)   | 26 (1.41%)      | 42 (1.52%)   | 226 (1.2%)   |
| Average OSRs length                     | 3.26 +/- 2.74 <br> min. 1 <br> max. 26   | 3.69 +/- 3.24 <br> min. 1 <br> max. 27      | 4.00 +/- 3.65 <br> min. 1 <br> max. 24   | 3.65 +/- 3.21 <br> min. 1 <br> max. 25.7   |
| Number of sentences with negated statements | 5,631    | 755         | 1,134   | 7,520    |
| Number of multiword negation cues       | 540      | 63          | 108     | 711      |
| Number of discontinuous negation cues   | 4        | 0           | 1       | 5        |
| Number of sentences with multiple negation cues | 954 (6.9%)   | 119 (6.47%)      | 204 (7.38%)   | 1,277 (6.93%)   |
| Average negation cue length             | 1.09 +/- 0.32 <br> min. 1 <br> max. 7   | 1.08 +/- 0.30 <br> min. 1 <br> max. 5      | 1.08 +/- 0.31 <br> min. 1 <br> max. 5   | 1.08 +/- 0.31 <br> min. 1 <br> max. 5.7   |
| Number of sentences with negation scopes | 5,138    | 696         | 1,045   | 6,879    |
| Number of multiword negation scopes     | 4,684    | 585         | 992     | 6,261    |
| Number of discontinuous negation scopes | 11       | 2           | 3       | 16       |
| Number of sentences with multiple negation scopes | 873 (6.31%)   | 106 (5.76%)      | 192 (6.94%)   | 1,171 (6.35%)   |
| Average negation scope length                 | 3.92 +/- 3.46 <br>min. 1<br>max. 42 | 3.83 +/- 3.86 <br>min. 1<br>max. 49 | 3.96 +/- 3.53 <br>min. 1<br>max. 36 | 3.90 +/- 3.62 <br>min. 1<br>max. 42.3 |
| Number of sentences with uncertainty statements | 1,620                        | 223                          | 332                          | 2,175                       |
| Number of multiword uncertainty cues           | 700                          | 95                           | 156                          | 951                         |
| Number of discontinuous uncertainty cues       | 0                            | 0                            | 0                            | 0                           |
| Number of sentences with multiple uncertainty cues | 196 (1.42%)                | 27 (1.47%)                   | 49 (1.77%)                   | 272 (1.47%)                 |
| Average uncertainty cue length                 | 1.42 +/- 0.59 <br>min. 1<br>max. 7 | 1.39 +/- 0.53 <br>min. 1<br>max. 4 | 1.42 +/- 0.53 <br>min. 1<br>max. 3 | 1.41 +/- 0.55 <br>min. 1<br>max. 4.7 |
| Number of sentences with uncertainty scopes     | 1,616                        | 221                          | 328                          | 2,165                       |
| Number of multiword uncertainty scopes          | 1,536                        | 210                          | 327                          | 2,073                       |
| Number of discontinuous uncertainty scopes      | 11                           | 2                            | 1                            | 14                          |
| Number of sentences with multiple uncertainty scopes | 207 (1.5%)                 | 26 (1.41%)                   | 49 (1.77%)                   | 282 (1.53%)                 |
| Average uncertainty scope’s length    | 5.05 +/- 4.96<br>min. 1<br>max. 42 | 5.48 +/- 4.97<br>min. 1<br>max. 40 | 4.71 +/- 4.12<br>min. 1<br>max. 24 | 5.08 +/- 4.68<br>min. 1<br>max. 35.3 |
