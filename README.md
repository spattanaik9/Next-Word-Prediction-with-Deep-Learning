# Next-Word-Prediction-with-Deep-Learning
This project implements a Next Word Prediction model using deep learning techniques and TensorFlow. The goal of this project is to develop a language model that can predict the most likely word to follow a given input sequence of words, making it a valuable tool for various natural language processing (NLP) applications.

Task:
This project is on language modeling for an artificial language. We want to build a model such that given a "partial text" in the artificial language, the model can predict the next word.

As a training dataset, a list of 5,000 texts in the artificial language are here. (After downloading it, you can use pickle.load(open(path,'rb')) to open it. It is a list of 5,000 strings in Python. For example, a string may be 'a j a d a d c g b f a i c f b e a e a h b e a d c d c d c d b d c f '.)

From the above 5,000 strings, we have obtained 5,000 "partial texts" and the corresponding "next word". Each "partial text" consists of the first k words of the corresponding string (for some random integer k), and the corresponding "next word" is the (k+1)-th word in that string. For example, for the string 'a j a d a d c g b f a i c f b e a e a h b e a d c d c d c d b d c f ', the "partial text" may be ['a', 'j', 'a', 'd', 'a', 'd', 'c', 'g', 'b', 'f', 'a', 'i', 'c', 'f', 'b', 'e', 'a'], which is a list of the first k=17 words in the string, and the "next word" is 'e', which is the 18-th word in the string.

Your task is to design and train a good model, which takes "partial texts" as input, and predicts the "next word" for each "partial text".

Your trained model will be evaluated using a "testing dataset" (shown below). The testing dataset also consists of a list of "partial texts" (as the model's input) and a list of "next word" (to be compared to your model's output). In the list of "partial texts", each "partial text" is a list of words instead of a single string, just like the "partial texts" above that we have for the training set. The performance of your model will be measured by its "accuracy for words", defined as the fraction of "next words" that your model correctly predicts.

As the "testing dataset" for this project, a list of 5,000 "partial texts" are here. Please run your trained model on it to get the 5,000 corresponding "next word" (as a list of 5,000 strings in Python) 

