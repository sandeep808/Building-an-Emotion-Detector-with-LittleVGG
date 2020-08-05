# Building-an-Emotion-Detector-with-LittleVGG

Our Facial Expression Dataset :

● Our dataset is hosted on Kaggle and has been around since 2013.

● It consists of 28,709 examples of faces showing the 7 followingexpressions

1.Angry 
2.Happy 
3.Neutral
4.Disgust
5.Sad
6.Fear
7.Surprise

but in building the model, i have deleted the disgust class as there are too few images.
so, i build the model using 6 classes.

● Our images are grayscale and 48 x 48 pixels


Approach : 

● Use our LittleVGG model with the following changes

○ Swapping ReLU activations for ELU

○ Changing our initializations from Kera’s default Glorat Normal to He Normal (tends to work better for VGG type Networks)

● We then use OpenCV with a HAAR Cascade Classifier trained on faces, to extract our face from our webcams and classifier our emotions in real time!
