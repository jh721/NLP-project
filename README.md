# NLP-project

topic: musical instrument classification


# Mel spectrogram
def get_melspectrogram: converting an audio file to a Mel spectrogram


# data augmentation on wave file
def add_noise
def shift_time
def change_pitch
def stretch_time

#data augmentation on Mel spectrogram
def time_masking
def freq_masking


#make IRMAS-TrainingData
make soundwaves and corresponding labels to a dataset into a format easy to use


#make test set
seperate test set in the beginning, SHOULD NOT BE TOUCHED AGAIN WHILE RUNNING CODE


#saving blocks
since converting to melspectrogram takes long time, save it in advance


#train_val set augmentation
extend dataset with augmented data


#shuffle dataset
shuffle the extended dataset to give randomness


#make train, val set
split into several pieces to use with (k-fold) cross validation


#Model
construct model referring to the research paper


#training
def model_train
def model_train_cross_val: repeat model_train with each train and val set, output the model with lowest validation loss


#test
def test_model: output model accuracy with test dataset


#run model
set loss function as crossentropyloss
set optimizer as ADAM


#save and load model
for later use save trained model
