# Gesture-Controlled-VLC-Media_Player
Gesture Controlled Media Player that recognizes hand gestures.
Supported Gestures: <br>
1.Swipe Left -> Forward by 10 seconds <br>
2.Swipe Right -> Rewind by 10 seconds <br>
3.Stop Sign -> Mute <br>
4.Drumming fingers -> Play/Pause <br>
5.Zooming In with Hand -> Switch to Full Screen/ Exit Full Screen <br> 

About:
The project uses a ML Model especifically Resnet-101, trained on 20bn-jester-v1 dataset (22.8 GB)(Link-https://20bn.com/datasets/jester).<br>
The model is able to classify 27 different Hand Gestures whose can be found on the above link.<br> 
The predictions made by the model are then linked with keyboard which simulates pressing of keys coressponding to a particular gesture.<br>
This project can be extended to Gesture Controlled Powerpoint Slides, Word, simple game controls and various other processes. <br>
The model accuracy is 93% on validation data and 99% on train data. 
