**Ishihara Test Image Segmentation**
This repository provides a Python implementation for segmenting and analyzing** Ishihara test images using K-Means clustering**. The goal is to help isolate the number or symbol embedded in Ishihara plates, commonly used for color vision deficiency testing. The code is designed to run in Google Colab and leverages libraries such as NumPy, Matplotlib, and PIL.
 
Features
•	Upload and process Ishihara test images directly in Colab.
•	Custom K-Means clustering implementation for image segmentation.
•	Visualizes both the original and segmented images, along with a color palette of detected clusters.
•	Interactive selection of clusters to isolate and highlight the embedded number/symbol.
•	Outputs a binary image with the number highlighted in red on a black background.
 
**How It Works**
1.	Image Upload:
Upload an Ishihara test image using the Colab file upload widget.
2.	Segmentation:
The image is segmented into k color clusters using a custom K-Means algorithm.
3.	Visualization:
The script displays:
o	The original image.
o	The clustered (segmented) image.
o	The color palette representing each cluster.
4.	Cluster Selection:
The user is prompted to input which cluster(s) correspond to the number in the Ishihara plate.
5.	Number Isolation:
The selected clusters are highlighted in red, isolating the number against a black background.
 
Usage
Requirements
•	Python 3 (recommended in Google Colab)
•	Libraries: numpy, matplotlib, PIL
Steps
1.	Clone the Repository: 
git clone https://github.com/MohamedKemo1350/Ishihara-Test-

cd Ishihara-Test-

2.	Open the Notebook
o	Open Ishihara_Test.ipynb in Google Colab for the best experience.
3.	Run the Notebook
o	Execute the cells in order.
o	When prompted, upload your Ishihara test image.
o	Enter the cluster indices that represent the number when asked.
 
Code Structure
Function	Description
KMeans	Custom K-Means clustering class
load_image_colab()	Handles image upload in Colab
segment_image()	Segments the image into k clusters
visualize_clusters()	Displays original, clustered images, and color palette
isolate_number()	Prompts for cluster selection and isolates the number
extract_red_number_image()	Main function to run the workflow and display results

 Example Output
•	Left: Original Ishihara image
•	Right: Isolated number in red
 
Customization
•	Adjust the number of clusters (k) in extract_red_number_image(k=19) for different images.
•	The code is modular and can be extended for batch processing or automated cluster selection.
 
•	Built using open-source Python libraries.
 
Contact
For questions or suggestions, please open an issue or contact MohamedKemo1350.
 

