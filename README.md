# Brain-Tumor-detection
The dataset contained
a total of 3929 Magnetic Resonance Imaging images that were
used to implement the approach where at first, data generator
and augmentation were done, and then the models were trained
on large data sets after which tumor was segmented.To eval-
uate which model performance is better concerning dice co-
efficient and IoU were used and, the same was the best for
unet with values 0.93 and 89 percent.

# Source of dataset
uses Kaggle dataset,![dataset](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection)This dataset contains brain
MRI images together with manual FLAIR abnormally seg-
mentation masks.These images were obtained from the Cancer
imaging Archive(TCIA).There are a total of 3929 images and
its masks.The data set did not contain any human participant
or any sensitive data that could break any legal or ethical rules.
Data sets were gathered from ‘Cancer Imaging Archive’ for
this implementation. All the files were in the form of .tif for-
mat. Out of the total 7863 files, 2 files represented the values of
the tumor which were in the form of .csv file.86 MRI were du-
plicates.This data set was a combination of MRI

# Methodology
A machine Learning model is quite is relevant for everyone
operating on it. In brief, the brain MRI images and their cor-
responding tumor masks generated using manual segmentation
were proposed and then used for for training the segmentation
model. The trained segmentation model and the processed MRI
images were then used to automatically generate tumor masks
. The grading model used a sub-set of the processed MRI im-
ages based on the generated tumor masks for classifying im-
ages with different grades.
The first step is to crop unnecessary regions that correspond
to non tissue areas from the MRI and the corresponding tu-
mor mask images for all images of each patient. The cropping
was performed in three dimensions of images per patient (i.e.,
height, width, and elevation –image slices)
# Unet
U-Net is a convolutional neural network that was developed for biomedical image segmentation at the Computer Science Department of the University of Freiburg.[1] The network is based on the fully convolutional network[2] and its architecture was modified and extended to work with fewer training images and to yield more precise segmentations. Segmentation of a 512 × 512 image takes less than a second on a modern GPU.
   
 # Result
![image](https://user-images.githubusercontent.com/65977290/125761439-082dc773-1a92-4c36-bee7-d2a56ddba89e.png)

