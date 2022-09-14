# Glaucoma-Detection
Glaucoma is a disease that damages your eye’s optic nerve. It usually happens when fluid builds up in the front part of your eye. That extra fluid increases the pressure in your eye, damaging the optic nerve, which may lead to vision loss or even blindness. 

Fundus photography is the process of taking serial photographs of the interior of your eye through the pupil. A fundus camera is a specialized low-power microscope attached to a camera used to examine structures such as the optic disc, retina, and lens.

Glaucoma can be detected through cup-to-disc ratio(CDR).
CDR is the ratio between optic disc and optic cup.
CDR can be found by feature extraction of the optic nerve head by machine learning techniques.
A person diagnosed with Glaucoma usually has a CDR value greater than 0.5.

Below are the main Modules for Glaucoma Detection used in this project:
Optic Disc Localization
Optic Disc and Cup Segmentation
Glaucoma Feature Extraction
Classification

LOCALIZATION:
Intensity variations in the image can help locate the optic disc in fundus images. Localization is to segment the image into various objects in order to find the brightest object of the image, which is located in the optic cup (OC) and, hence, is a part of the OD. The disc center is marked at the point where the highest intensity is found. 

SEGMENTATION:
Segmenting the optic disc (OD) is an important and essential step in creating a frame of reference for diagnosing Glaucoma. Therefore, a reliable OD (optic disc) segmentation technique is necessary for the automatic screening of optic nerve head abnormalities. 
Here, we used the following segmentation techniques for feature extraction:
Circular Hough transform Model fitting
Ellipse fitting

CLASSIFICATION:
This module of the project classifies the the given fundus images as either glaucoma or normal eye by inferencing the fundus images after performing all the above techniques on the fundus images.

HOW TO RUN THIS CODE?
Below are the procedure for using this script:

Run this: python inference_script.py in command prompt. Make sure you are in 'Code' directory.
Choose your retinal image.
After a few seconds, the detection result should appear in command prompt and json file.








