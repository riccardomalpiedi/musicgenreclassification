# Music genre classification project for NAML exam

For this project we used as a reference the work of Bisharad and Laskar (https://onlinelibrary.wiley.com/doi/10.1111/exsy.12429).

## Data

The dataset we used is GTZAN (https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification) and it is composed of 1000 extracts of 30 seconds of songs belonging to 10 different genres (100 songs for each genre). We computed the melspectrograms of all the samples and we used them to train and test our neural network. You can see a plot of a melspectrogram by running "mel_spectrogram.ipynb". The repository contains only the audio files, but by running "create_dataset_30sec.ipynb" you can get a file that contains the melspectrogram of each sample ("X_train") and a file that contains all the respective labels ("y_train"). The experiments were performed with 3000 extracts of 10 seconds, you can generate the dataset by running "create_dataset_10sec.ipynb".

## Experiments

The notebooks "music_genre_classification.ipynb" and "music_genre_classification_30sec_CCN+GRU.ipynb" contain the code to load and reshape the data, train the respective models (a CNN model and a CNN model with a GRU layer at the end) and evaluate them.
