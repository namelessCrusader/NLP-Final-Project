# NLP-Final-Project

This repository is a part of the Deliverables for our final project for CS6120 - NLP.

The dataset(Sentiment Analysis with Financial News) we use is from [Kaggle](https://www.kaggle.com/code/venomsnake/sentiment-analysis-with-financial-news/input).
It has 5322 amount of samples, out of which 2874 are positive, 1703 are negative and 798 are neutral.
We remove escape sequences, stop words, links, out of vocabulary words, and words with less than 2 characters. 
Because we remove all words not in the vocabulary, we do not explicitly handle words of that class. But that can easily be handled by adding an Unknown token representing all words not in the vocabulary.

The code for pre-processing the dataset exists in the iPython notebook.

The way our iPython notebook is structured, we used a T4 GPU available on Google Colab for training the RNNs and trained the BERT model locally.

In order to re-run the tests for LSTMs:
1. Upload the dataset to the base Google Drive Directory
2. Link your Google Drive to Google Colab
3. Run all cells leading upto the test. 

In order to re-run the tests for BERT:
1. If you are locally running it, keep the iPython notebook in the same directory as the notebook.
2. Or place the dataset in the core working directory of Google Colab if you wish to use it.
3. Run all cells from the title of Transformer leading upto the test.

The cell outputs have been wiped for code readability purposes. 

The project report can be found [here](https://drive.google.com/file/d/1win-9LBOucD8JHj-FJlk1rBCK-uwxpD9/view?usp=sharing) and uploaded to this repository.
