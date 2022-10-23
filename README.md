# Lafz, an Automated Speech Recognition System  (ASR) for Urdu
Lafz is a speech-to-text conversion tool for the Urdu language, developed as part of our semester project, using the Kaldi toolkit. The program uses Automated Speech Recognition technology and logic to train over a small dataset and then extends its functionality to new, similar audio files, previously untrained on. For now, Kaldi B Urdu is limited to listening to pre-recorded wav files and generating corresponding Urdu text, however, it can further be extended to convert speech to text in real time.

##### A full report related to this project, with complete on-paper details, can be found in the source files.

We were able to successfully train our model on four out of the six chosen training models and achieved an accuracy of approximately 79-81%. etails about these models can also be found in the report attached.

It can be seen that training the model on monophones only gave us an accuracy of 66.81% but the accuracy dramatically increased to 81.01% once we were done training on Tri1. However the slight decrease is accuracy after training our model on Tri2 and Tri3 is slightly confusing for us right now. For now, we cannot say for sure, but we hope that extending the training to SGMM2 and MMI-SGMM2 would overcome this deficiency and increase the accuracy.

The results of newly recorded sentences show that the model is pretty accurate on decoding sentences which use the words which already exist in the dictionary. However, for words which do not exist in the model’s dictionary, the accuracy is slightly lower. The model still decodes it to some similar word though, like it decoded the word ‘daant’ to ‘daad’ since the former didn't exist in the dictionary. We are hopeful that extending the training set to a larger dictionary might help us resolve this issue.

#### Lafz itself has been coded in Python, using Kaldi toolkit, on Google Colab.
