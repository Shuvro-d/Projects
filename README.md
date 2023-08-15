# Projects

100 -> program for generating confusion matrix from the output of the model and their labels for yolov5 and yolov7

101-> This project involves Lung segmentation from X-ray images using Unet architecture. The dataset is collected from Kaggle and the purpose of this project was to understand semantic segmentation using U-Net architecture.

102-> This project is similar to the previous project. Here I segmented Kidney from CT images. The images are collected from GitHub and I annotated every image using label-studio to create the binary mask. Then I trained the model.

103-> This project is done using both U-net and autoencoder architecture. First I annotated the data and because very few data are available the IOU of the U-net model is very low. So, I tried to improve the IOU by first generating a pre-trained weight using the Autoencoder and then training the U-net model. The purpose was to learn how to generate a pre-trained weight using the Autoencoder.

104-> In this project I used the Double U-net model to segment brain tumors from MRI images. The dataset is collected from Kaggle and the main challenge was to write new metric functions to calculate the dice score, IOU, and accuracy as the previous functions of U-Net were not compatible with double U-Net. 

105-108-> These projects were done to learn how to train U-Net using pre-trained models of Imagenet (inceptionv3, vgg16 and resnet34) as backbone and compare their metrics to find out which works better with U-Net.

109-113-> This project involves the classification of different types of brain tumors using Random forest with and without pre-trained models.

114-115-> This project involve Teal Leaf Disease detection using YOLOV5 and YOLOV7 algorithm. The dataset was provided by my supervisor and I annotated them and trained them for him to see my accuracy are similar to his or not.

117-> This project is segmenting brain tumor using Attention Unet.

119-> This project is segmenting brain tumor using transoformer Unet.

120-123-> This project involves image classification using support vector machine and YOLO algorithm.


