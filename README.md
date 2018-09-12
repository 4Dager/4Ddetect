Requirements

    -cuda9.1
    -cudnn v7.1
    -opencv<=3.4.0
    
Install
    
    git clone https://github.com/4Dager/vSlam-Perspective.git
    
Pre-trained models for different cfg-files can be downloaded from (smaller -> faster & lower quality):

    baiduyun
    
Compile

&nbsp;
Open build\darknet\darknet.sln, set x64 and Release, then build with Microsoft Visual Studio 2015. Then open build\darknet\x64 and perform the following in cmd:

    darknet detector test cfg\coco.data cfg\yolov3.cfg yolov3.weights data\dog.jpg

Then you can get the predictions of the data\dog.jpg