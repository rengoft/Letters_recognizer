# Letters_recognizer
## The problem to be solved.
The work is devoted to the recognizing handwritten russian alphabet letters. The letters are taken from three datasets. One of them contains 
colored photographs of letters written down in a [school copybook (School_paper_letters.zip)](School_paper_letters.zip). Two other datasets are 
[CoMnist_letters.zip](CoMnist_letters.zip) and [NoName_letters.zip](NoName_letters.zip))
are composed of binary black-and-white pictures.
## Solution
The letters recognizing is performed in three ways. In one way the structure of a letter is analysed and features of the letter structure model are taken. To form the feature vectors method of crosses is used. Also features are formed via calculating a mean pixel number of the letter structure model lying on rows, columns and main diagonals of the model image. These letters processings are performed in [data_prep.ipynb](data_prep.ipynb). Then, the obtained feature vectors are passed to [supporting vectors machine](ml_classifiers.ipynb) and to [fully connected neural network](keras_nn_model.ipynb).
Additionally, the images of the letters themselves are used to train convolutional networks which is realised in the files [CNN_pictures.ipynb](CNN_pictures.ipynb) and
[CNN_Kaggle_School.ipynb](CNN_Kaggle_School.ipynb).
