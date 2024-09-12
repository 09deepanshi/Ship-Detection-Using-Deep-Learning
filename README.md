Hello everyone,

Here is my project in the field of Computer Vision, focusing on Satellite Ship Detection using Deep Learning techniques. In this project, we work with the Airbus dataset, which contains 1,960,389 training images, each accompanied by a respective mask.

The project is divided into three major parts:

Generating the Masks using Run Length Encoding (RLE):
The first step involves generating masks for the images by decoding the RLE format, which is essential for locating the ships in each image. We decode the encoded ship regions and generate masks accordingly.

Preparing the Training and Validation Data:
Since a significant portion of the dataset consists of images that do not contain ships, we perform random undersampling to balance the data. Additionally, we preprocess the images by flattening them and creating segments. We also apply data augmentation, which includes flipping, rotating the images, and adjusting the brightness levels. This helps in improving the robustness of the model.

Building and Training the U-Net Model:
As we are performing image segmentation, we use the U-Net architecture, which is well-suited for this task. The pre-processed data is fed into the U-Net model for training. After training, we validate the model by testing it on random images from the dataset to check whether it is correctly segmenting and detecting ships in satellite images.

Through this approach, we can effectively segment the images, identifying whether a ship is present or not with high accuracy.

This version clearly explains the steps in your project, while maintaining a professional and informative tone.
