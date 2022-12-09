# Projects

This projects are done for learning purpose. Most of the codes are collected from different tutorials. Some datasets were created by me and others are collected from different sources. I tried to mention all the resources I used. 


->Confusion matrix for test data in YOLOv5 and YOLOv7

To get the confusion matrix for Yolov5 and v7, First You need to create a folder name test data and inside the folder create two additional folder named positive and negative. Where the images on those the Yolo will detect objects will be kept on positive folder and on those Yolo won't detect anything will be kept on negative folder.
Then instead of using the detect.py function use the confusion_matrix_for_test_data.py or you can rename the file as you like and for test data location use the test data folders location not positve or negative folder. The commands will be like this-

For v5
!python confusion_matrix_for_testdata_v5.py --weights best.pt  --img 640 --conf 0.5 --source  /content/test_data

For v7 
!python confusion_matrix_for_testdata_v7.py --weights  best.pt  --conf 0.5  --img-size 640 --source /content/test_data

The code is just little changed from the original detect.py file from YOLO repository. You can find the original Yolo repository here
https://github.com/ultralytics/yolov5
https://github.com/WongKinYiu/yolov7








->Lung segmentation: 

In this project I tried to segment the lung from x-ray chest images. The data set has almost 600 x-ray images  and corresponding masks. UNET architecture is used for sematic segmentation. dataset: https://academictorrents.com/details/ac786f74878a5775c81d490b23842fd4736bfe33








->Kidney segmentation:

In this project I tried to segment the lung from CT images. The data set has almost 1600 CT images  and corresponding masks. The CT images are collected from https://github.com/Shuvro-d/Kidney_stone_detection/tree/main/Dataset  . To create the masks I used label-studio. UNET architecture has been used for semantic segmentation.








->Skull segmentation:

Similar to the other projects UNET architecture is used for semantic segmentation. But here I also implemented autoencoder. Then I compared the outputs between two trained models. Where the first model is trained with pre-trained weights. Auto encoder is used for pre-training. Then the pre-trained weight is used for the UNET models training. The other model is Trained with random weight just like the other semantic segmentation project. We can see how the IOU increased with the pre-trained weights.
The images for the dataset were provided by my thesis supervisor and the masks were created using label-studio. 
dataset: https://drive.google.com/drive/folders/1U8b-nHynpibcGAO6u2YRqL9fRxpyixUl?usp=sharing
