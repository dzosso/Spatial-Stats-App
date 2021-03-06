# Spatial-Stats-App
* App used to locate dendritic cell nuclei in images of gastric mucosa.
* Then computes several statistics of the images and compares them to simulated data.

## Installation:
* For all browsers, download dendritic_segmentation_Integration_exported.m
* Log into MATLAB Online on a Chrome browser and upload the .m-file to your MATLAB online repository.
* Upload the images and their associated Selection.csv files to your MATLAB online repository.
* For Chrome users, the dendritic_segmentation_Integration.mlapp file works; however, it is recommended that the dendritic_segmentation_Integration_exported.m file be used.

## Usage:
* Open the folder in your MATLAB repository in which you wish to save the generated MAT files to.
* Run the app be right clicking the dendritic_segmentation_Integration_exported.m file and clicking run.
* Click the "Select TIF" button and choose the desired TIF to be analyzed (contains the image data).
* Click the "Select CSV" button and choose the CSV corresponding to the TIF (contains the ROI information).
* Click the "Display TIF Channels" button to see each channel in the TIF.
* Set the "Nuclei Channel" and "DC Channel" spinners to the corresponding channels as seen in the TIF channels.
* (Blue should be the Nuclei Channel, Green should be the DC Channel, Red should be the Epithelium Channel)
* Click "Run" and note the figure generated is an overlay of the DC Channel (Green), Nuclei Channel (Blue), and located DC nuclei (Red).
* Ensure that a MAT file has been generated in your "Current Folder".
* Checking "debug" will generate intermediate figures of various parts of the image analysis when the app is run again.
* If necessary adjust the "Threshold" slider to more or less severe thresholding to get the correct MNP nuclei detection.
* If necessary adjust the "Disk Size" scroll bar for larger or smaller convolution disk radius to tune the MNP localization.
* Threshold values are between 0 and 1.
* Note figures can be closed individually, or all at once by clicking "Close Figures".

## Outputs:
* The program produces images as well as a MAT, CSV, and TXT file.
* The name of the MAT file and TXT will be the same as the selected TIF along with chosen threshold.
* The MAT file contains the ROI, found nuclear centers, and identified dendritic cells.
* The TXT file stores the chosen parameters, number of indentified nuclei, number of identified dendritic cells, and several statistics.
* The CSV files contain the observed cell-cell and cell-epithelium distances, and simulated c-c or c-e distances, respectively.

## Videos:
* OUTDATED Use this URL for a video tutorial on the MATLAB app: https://www.youtube.com/watch?v=1bb0FJu9tZc&feature=youtu.be
* Use this URL for an video overview of the Statistics Pipeline: https://www.youtube.com/watch?v=sl2b1jzobso&feature=youtu.be

