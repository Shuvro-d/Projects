# Projects

This projects are done for learning purpose. Most of the codes are collected from different tutorials. Some datasets were created by me and others are collected from different sources. I tried to mention all the resources I used. 


100->Confusion matrix for test data in YOLOv5 and YOLOv7

To get the confusion matrix for Yolov5 and v7, First You need to create a folder name test data and inside the folder create two additional folder named positive and negative. Where the images on those the Yolo will detect objects will be kept on positive folder and on those Yolo won't detect anything will be kept on negative folder.
Then instead of using the detect.py function use the confusion_matrix_for_test_data.py or you can rename the file as you like and for test data location use the test data folders location not positve or negative folder. The commands will be like this-

For v5
!python confusion_matrix_for_testdata_v5.py --weights best.pt  --img 640 --conf 0.5 --source  /content/test_data

For v7 
!python confusion_matrix_for_testdata_v7.py --weights  best.pt  --conf 0.5  --img-size 640 --source /content/test_data

The code is just little changed from the original detect.py file from YOLO repository. You can find the original Yolo repository here
https://github.com/ultralytics/yolov5
https://github.com/WongKinYiu/yolov7








101->Lung segmentation: 

In this project I tried to segment the lung from x-ray chest images. The data set has almost 600 x-ray images  and corresponding masks. UNET architecture is used for sematic segmentation. dataset: https://academictorrents.com/details/ac786f74878a5775c81d490b23842fd4736bfe33








102->Kidney segmentation:

In this project I tried to segment the lung from CT images. The data set has almost 1600 CT images  and corresponding masks. The CT images are collected from https://github.com/Shuvro-d/Kidney_stone_detection/tree/main/Dataset  . To create the masks I used label-studio. UNET architecture has been used for semantic segmentation.








103->Skull segmentation:

Similar to the other projects UNET architecture is used for semantic segmentation. But here I also implemented autoencoder. Then I compared the outputs between two trained models. Where the first model is trained with pre-trained weights. Auto encoder is used for pre-training. Then the pre-trained weight is used for the UNET models training. The other model is Trained with random weight just like the other semantic segmentation project. We can see how the IOU increased with the pre-trained weights.
The images for the dataset were provided by my thesis supervisor and the masks were created using label-studio. 


104->Brain Tumor segmentation using double U-Net

In this project I just used double U-Net instead of regular U-Net to segment brain Tumor from MRI images. The dataset is downloaded from kaggle and it contains 3000 images and 3000 masks.



105-107->Pre training U-Net with vgg, resnet and inception

In this projects I used vgg, resnet and inception to pre-train the U-Net so that U-Net uses pre-trained weight in the encoder instead of random weight to increase the performance of the model. It is similar to autoencoder that I implemented in project 103.


108->Comparison of vgg, resnet and inception

In this project I compare the three backbones, how they improve the performance of the U-Net model. Instead of manually implementing I used segmentation-models library to call the models and evaluated which backbone is the best.


109->Brain-Tumor classification

In this project I used the Random-Forest algorithm to classify pituitary, meningioma and glioma tumor types.

110->Classification of mri planes

In this project I used the Random-Forest algorithm to classify axial, coronal and sagittal plane types.


111-113->Random forest with backbones.

Similar to U-net I used vgg, resnet and inception to extract features from images before training the random forest algorithm.

114-115>Tea leaf disease detection using YOLO algorithm

I used YOLOv5 and YOLOv7 to detect red spider, leaf rust, tea-mosquito bite, brown blight, black rot and white spot disease. The dataset was provided by my supervisor which was collected from malanichara tea garden, sylhet.


116-> Classification with xgboost

In this project I classified brain tumor using xgboost. Similar to random forest.
