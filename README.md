# Projects

This projects are done for learning purpose. Most of the codes are collected from different tutorials. Some datasets were created by me and others are collected from different sources. I tried to mention all the resources I used. 

->Lung segmentation: 

In this project I tried to segment the lung from x-ray chest images. The data set has almost 600 x-ray images  and corresponding masks. UNET architecture is used for sematic segmentation. dataset: https://academictorrents.com/details/ac786f74878a5775c81d490b23842fd4736bfe33


->Kidney segmentation:

In this project I tried to segment the lung from CT images. The data set has almost 1600 CT images  and corresponding masks. The CT images are collected from https://github.com/Shuvro-d/Kidney_stone_detection/tree/main/Dataset  . To create the masks I used label-studio. UNET architecture has been used for semantic segmentation.

->Skull segmentation:

Similar to the other projects UNET architecture is used for semantic segmentation. But here I also implemented autoencoder. Then I compared the outputs between two trained models. Where the first model is trained with pre-trained weights. Auto encoder is used for pre-training. Then the pre-trained weight is used for the UNET models training. The other model is Trained with random weight just like the other semantic segmentation project. We can see how the IOU increased with the pre-trained weights.
The images for the dataset were provided by my thesis supervisor and the masks were created using label-studio. 
dataset: https://drive.google.com/drive/folders/1U8b-nHynpibcGAO6u2YRqL9fRxpyixUl?usp=sharing
