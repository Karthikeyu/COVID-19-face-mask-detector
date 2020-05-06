# COVID-19-face-mask-detector
Hi, this repository contains python implementation for face mask detection using python, deep learning, keras and tensorflow.
It uses MobiNetV2 network model using fine tuning with pretrained [ImageNet](http://www.image-net.org/) weights. The reason for using this model is; it is light weight low processing and can be used with low end embedded devices. This is implemented from [pyimagesearch](https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/) blog. The data set is obtained from [prajna bhandary's repository](https://github.com/prajnasb/observations/tree/master/experiements/data). How ever the dataset is artificially made, I would like to add original images with mask instead of facial land mark applied dataset so that it would be more robust and accurate. 

## The required libraries:

* > pip install opencv 
* > pip install tensorflow
* > pip install keras
* > pip install argparse
* > pip install imutils

## Steps to run:

* Run the file **train_mask_detector.py** and enter following command  (It trains the MobinetV2 and predicts the accuracy for test data)
> python train_mask_detector.py --dataset dataset
*  Run the file **detect_mask_image.py** to detect mask from static images (replace example_01.png with your image)
> python detect_mask_image.py --image examples/example_01.png 
* Run the file **detect_mask_video.py** to detect from video stream
> python detect_mask_video.py

Credits:
* [PyimageSearch blog Adrian](https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/) 
