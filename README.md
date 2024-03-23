# Semantic Segmentation
In this project, a study was conducted on lightweight model, focusing specifically on MobileNet. Semantic segmentation was performed using the MobileNet model on two popular datasets: CamVid and Stanford Background Dataset.

Dataset:

CamVid: This dataset consists of images captured from a vehicle-mounted camera while driving in urban areas. It includes pixel-level annotations for various semantic classes such as road, pedestrian, car, etc.

Stanford Background Dataset: This dataset contains images with pixel-level annotations of outdoor scenes. It is commonly used for semantic segmentation tasks.

Files:

1)SemSeg.ipynb:
This notebook contains the implementation of image semantic segmentation using MobileNet on theStanford dataset. It includes preprocessing steps, model training, evaluation, and visualization of segmentation results.

2)Mobilenet_for_videosegmentation.ipynb:
This notebook demonstrates video semantic segmentation using MobileNet. It provides a step-by-step guide on preprocessing video data, applying semantic segmentation to each frame, and generating segmented videos.


For comparing the model's performance, two comparison metrics were used namely Dice Loss and mIoU (Mean Intersection over Union) score.
a) mIoU is computed by taking the average of the IoU scores across all classes in the 
segmentation task. It provides an overall measure of the model's performance in segmenting 
multiple classes.
mIoU = (IoU1 + IoU2 + ... + IoUN) / N (1)

b) Dice Loss is a loss function which is designed to address class imbalance and encourage 
accurate segmentation at the pixel level. It penalizes the model for low overlap and rewards 
accurate segmentation.
Dice Loss is given by:
Dice Loss = 1 - Dice coefficient (2)
Where Dice Coefficient (also known as F1 Score) is the ratio of twice the intersection of the 
predicted and ground truth masks to the sum of their areas
Dice coefficient = (2 * Intersection) / (Ground Truth + Predicted) 

**MobileNetV3 Performance:**

mIoU Score: 0.446

Number of Epochs: 75

Training Time: 45 minutes

Dice Loss: 0.503
