=>  The idea of this task was to find individual probabilities for each word. These probabilities were summed for all the words extracted from the doc. The language with highest cumulative probability was 	declared to be the major one.

=>  The task was implemented by two methods- 

		1. Neural network method where characters of the word were vector encoded and the resultant vectors were aligned together to vector encode each word. A Neural Network classifier was trained, which gave 95% accuracy on validation set.

		2. Word Embedding method- Words extracted from the dictionary were tokenized and their embeddings was calculated. Those embeddings were then passed on to a neural network classifier. This method gave 93% accuracy on the validation set.

=>  The dataset is highly flexible and new languages can be added and data size can be increased very easily. The model is initially built for three languages- English, German and French. Its predictions 	get better with an increasing document length. For adding more languages or data, please refer to usage instructions.

=>  Usage Instructions-

	1. Since I was having hardware constraints, I used google colab. Please upload the file of respective method to 'home' of your    google drive
	2. To add more languages and/or increase data for any language-
		1. In nn_method make changes in config.py then run data_prep.py. Then run the notebook
		2. In embedding_method. Just make changes in config.py and then run the notebook 
	3. In each of the method add the text in "test.txt" file to find out its language
