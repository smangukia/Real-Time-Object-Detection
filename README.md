# Real-Time-Object-Detection
This is a custom object detection project created in jupyter notebook using TensorFlow Object Detection API and trained on pretrained model such as SSD MobileNet V2 FPNLite 320x320 from TensorFlow model zoo for intializing the custom model when training on novel datasets.
Built this project after learning from the TensorFlow Object Detection course online.

![rttfod3](https://user-images.githubusercontent.com/44052764/175282003-61fa42a8-9d99-41a5-b7d3-80cfe15f3c33.png)
## Steps  

**Step 1.** Clone this repository: https://github.com/smangukia/Real-Time-Object-Detection  

**Step 2.** Create a new virtual environment

             python -m venv rttfod  
            
**Step 3.** Activate the virtual environment

             .\rttfod\Scripts\activate # Windows  
            
**Step 4.** Install dependencies and add virtual environment to the Python Kernel

             python -m pip install --upgrade pip
            
             pip install ipykernel
             
             python -m ipykernel install --user --name=rttfod  
             
**Step 5.** Collect images using the Notebook 1. Image Collection.ipynb - ensure you change the kernel to the virtual environment
            As developed the virtual environment named rttfod, ensure that the upper right corner of your jupyter notebook has rttfod as the kernel  
            
**Step 6.** Manually divide the collected images into two folders train and test. So, now all the folders and annotations should be split between the following two folders.

             \TFODCourse\Tensorflow\workspace\images\train
            
             \TFODCourse\Tensorflow\workspace\images\test  
            
**Step 7.** Begin the training process by opening 2. Training and Detection.ipynb, this notebook will walk you through installing Tensorflow Object Detection, making detections, saving and exporting your model.  

**Step 8.** During this process the Notebook will install Tensorflow Object Detection. You should ideally receive a notification as OK in the last line, which means the Tensorflow Object Detection API has successfully installed.  

**Step 9.** Once you get to step 6. Train the model, inside of the notebook, you may choose to train the model from within the notebook. When training inside of a separate terminal on a Windows machine you're able to display live loss metrics.

**Step 10.** You can optionally evaluate your model inside of Tensorboard. Once the model has been trained and you have run the evaluation command under Step 7. Navigate to the evaluation folder for your trained model.  

             cd Tensorlfow/workspace/models/my_ssd_mobnet/eval  
            
and open Tensorboard with the following command

             tensorboard --logdir=.  
            
Tensorboard will be accessible through your browser and you will be able to see metrics including mAP - mean Average Precision, and Recall.           
