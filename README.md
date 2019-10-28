

# MapleStoryM-AutoQuest
Using Convolution Neural Network to identify current situation and click relative button to execute quest automatically.

The defualt path is `"C:\\Program Files\\Nox\\bin"` in `MapleM_AutoQuest_Model.ipynb` file.

## Note:
1. `MapleM_AutoQuest_double_InvecptionResNetv2.ipynb` is to train the image classification model using keras and tensorflow, it can be ignored if you just want to use the models that in [release](https://github.com/ChiHangChen/MapleStoryM-AutoQuest/releases).

2. `scenario` folder is my training data for training the deep learning model.

## Usage
1. Download two models (h5) files from [release](https://github.com/ChiHangChen/MapleStoryM-AutoQuest/releases).
2. Modify some variables : 
`
desired_window = "夜神模擬器"

# The Nox install path
path = "C:\\Program Files\\Nox\\bin"
os.chdir(path)

'''
The simulator default port, if you using multiple simulator, you should change the port.
You can check your port number use : os.popen('adb devices').read()
'''
print(os.popen('adb devices').read())
connect = os.popen("adb connect 127.0.0.1:62001").read()
print(connect)
`



3. Run the whole script `MapleM_AutoQuest_Model.ipynb`, it will catch screenshot frame by frame as model input and press relative position in Android simulator.

