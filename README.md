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
The model accuracy is 93% on validation data and 99% on train data.<br>

<b>Instructions:</b><br>
In order to use the application,follow the steps below:<br>
1. Download the repository as a ZIP and extract to your working directory<br>
2. Go to model folder and download the <i>resnetmodel</i> through the link provided in <i>info.txt</i><br>
3. Run <i>pip install requirements.txt</i><br>
4. Open jupyter notebook and run Classification.ipynb.<br>
5. Change the directory mentioned inside the load_model command, i.e. load_model(r"D:\20bn jester\model\resnet_3d_model\resnetmodel.hdf5") to load_model(r"Location where the downloaded model is kept"/resnetmodel.hdf5) and pd.read_csv(r"D:\20bn jester\jester-v1-labels.csv",header=None) to pd.read_csv(r"Your Working Directory/jester-v1-labels.csv",header=None).<br>
6. Run all the cells. <br>
7. Open VLC Media Player manually and the use the gestures as stated above. <br>


Future Updates:<br>
1. Remove the need of changing the directory in Classification.ipynb <br>
2. Remove the need of manually opening VLC Media player. <br>
