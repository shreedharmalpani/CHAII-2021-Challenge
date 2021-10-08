# Chaii-2021
This repositiory contains work done by us while trying for the Chaii-2021 challenge. For the challenge we have to design a model to predict answers for questions from articles written in Hindi and Tamil. To make this model we first started to learn and explore concepts about NLP and NLU. We learnt about transformers expecially BERT.   
We went through various articles and other resources to get an idea on how to proceed with this problem. Some of the really helpful articles were:
- https://towardsdatascience.com/nlp-building-a-question-answering-model-ed0529a68c54  
- https://medium.com/saarthi-ai/build-a-smart-question-answering-system-with-fine-tuned-bert-b586e4cfa5f5
- [A guide to transformers](https://towardsdatascience.com/illustrated-guide-to-transformers-step-by-step-explanation-f74876522bc0#:~:text=Encoder%20Layer&text=The%20Encoders%20layers%20job%20is,by%20a%20fully%20connected%20network.)   ( to learn about working of transformers)
- https://towardsdatascience.com/bert-explained-state-of-the-art-language-model-for-nlp-f8b21a9b6270 ( to learn more about how bert works)

We thought before moving on to Hindi and Tamil we should first try and make a model to predict answers to questions in English. So we used distilBERT( for faster training) to make a model to predict answers to questions from the Stanford question and answering dataset. This [train-v2.0.json](https://drive.google.com/file/d/1I5QpAss9_s4EzDTkYSk1q1OmBSkezW_N/view?usp=sharing) file is the training dataset from SQUAD that we used. The bert_qna.ipynb has the model that we implemented. 

We also tried to get word embeddings for hindi and tamil languages using BERT's word piece tokenizer itself. We directly [Chaii 2021's dataset](https://drive.google.com/file/d/1Bpkm_e5zsTQivFrkEt_hBSHdSi1QNWvq/view?usp=sharing) to train this on all the contexts given in the file.  The file Hindi_and_Tamil_Tokenization.ipynb contains this implementation. 

However we are also exploring google's Electra to use for pre training and generating word embeddings for Hindi and Tamil hoping to get better results. 
