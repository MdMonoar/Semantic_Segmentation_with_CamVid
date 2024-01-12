A Semantic Segmentation model was built through experiment also compared its performance against existing popular model UNet.

**Semantic Segmentation:**
<p align='justify'>
Image segmentation is a commonly used technique in digital image processing and analysis to partition an image into multiple parts or regions, often based on the characteristics of the pixels in the image. (mathworks.com)
</p>

<p align='justify'>
Image segmentation is an end-to-end image analysis process that divides a digital image into multiple segments and classifies the information contained in each region. The three kinds of image segmentation tasks—semantic, instance and panoptic segmentation—assign labels to individual pixels in the image to mark the specific boundaries and shapes of different objects and regions in the image, classifying them by using information like color, contrast, placement within the image and other attributes. (ibm.com)
</p>

<p align='justify'>
Semantic Segmentation is a process where every pixels of a specific class is labeled similarly and segmented together.
</p>

## About Data
A popular dataset named CamVid(Cambridge-Driving Labeled Video Database) was used for this project and was taken from popular data repository Kaggle. It consists of over 700 images and masks for semantic segmentation. The images and masks were seperated in training, validation and testing sets. The ground truth label associate each pixel with one of 32 semantic classes.

## KeyWords
- Sci-Kit Learn, NumPy, Pandas, Matplotlib
- TensorFlow, Keras, ImageDataGenerator
- ComputerVision, UNet

## Procedure
- Functions were built to mask training images according to labels
- Images were preprocessed keeping the resource limitations (gpu, memory etc.) in mind
- TensorFlow's ImageDataGenerator used to fit data optimally in the model
- A segmentation model was built and trained. Also the model was saved for later usage.
- Tested the performance the model, compared against existing architecture (UNet)
- Loaded the saved model to see if it functions like the original one.
