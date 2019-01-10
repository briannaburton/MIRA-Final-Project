# MIRA-Final-Project

Repository for the MIRA Final Project Challenge. Run ./src/Final_Project_Registration.ipynb in ./src/ to create elastix bash files, compute TRE, etc.  TRE results from experiments are found in ./registration-results/TRE-results.

### Pipeline for Challenge Day
1. Add images to ./data folder
2. Convert images from .img (raw format) to .nii.gz, being sure to change their orientation
3. Segment lung areas from exhale and inhale images and save as masks with "_mask" at the end
4. Add index & 300 to the original points .txt and add "_elastix" to the end of that file
5. Use ./src/Final_Project_Registration.ipynb to perform registration, point transformation, and to convert outputpoints.txt to a nparray and save in the original image folder in ./data with the extension "_transformed"
