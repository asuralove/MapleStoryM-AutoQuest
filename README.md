

# MapleStoryM-AutoQuest
Using Convolution Neural Network to identify current situation and click relative button to execute quest automatically.

Android PC simulator **Nox** install path must be defined!

The defualt path is `"C:\\Program Files\\Nox\\bin"` in `MapleM_AutoQuest_Model.ipynb` file.

## Note:
`MapleM_AutoQuest_double_InvecptionResNetv2.ipynb` is to train the image classification model using keras and tensorflow, it can be ignored if you just want to use the models that in https://github.com/ChiHangChen/MapleStoryM-AutoQuest/releases.

Download two model `h5` files from https://github.com/ChiHangChen/MapleStoryM-AutoQuest/releases and put and run whole script `MapleM_AutoQuest_Model.ipynb`, it will catch screenshot frame by frame as model input and press relative position in Android simulator.

