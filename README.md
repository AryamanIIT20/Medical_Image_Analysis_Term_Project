#### Corrections:
1. Symbol for space of Reals
2. Channels first instead of channels last

### Medical_Image_Analysis_Term_Project <br>
### Spring Semester 2024
Python Implementation of U-Net and scSE (spatial and channel squeeze and excitation) block <br>
for improved segmentation of organs in the CHAOS Dataset. Methods obtained from <br>
A. G. Roy, N. Navab and C. Wachinger, "Recalibrating Fully Convolutional Networks With <br> Spatial and Channel “Squeeze and Excitation” Blocks," in IEEE Transactions on Medical Imaging, vol. 38, no. 2, pp. 540-549, Feb. 2019, doi: 10.1109/TMI.2018.2867261.

### Data preparation
#### Masks
Binary masks were available for the CT images. For the multi-organ segmentation of MR images <br>
the binary masks for each organ were stacked channel wise to create one-hot encodings <br>
These were then converted to a single channel mask with integer labels.<br>
Approximate pixel ranges for labels are: <br>
Liver: 55-70 <br>
Right Kidney: 110-135 <br>
Left Kidney: 175-200 <br>
Spleen: 240-255 <br>
These were converted to integer labels in $[0,1,...4]$, 4 representing the background class
#### Images
DICOM images were scaled to uint8 representation <br>

The dataset is public at https://zenodo.org/records/3431873 <br>
The preprocessed dataset is available at https://drive.google.com/drive/folders/1JMtJm5mNArOx4_WUlrRXp5xUXaJq-_IH?usp=sharing <br>




Team Members: <br>
1. Aryaman Vikram Todi : 20EE38033
2. Aman Soni: 23EE65R02
3. Satyabrata Pradhan: 23EE65R20

