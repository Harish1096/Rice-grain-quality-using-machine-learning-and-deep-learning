											Rice Grain Quality Classification Using machine learning and Deep Learning
-License: MIT
	Python
	TensorFlow
	Flask
Automated multi-class classification of rice grains using Convolutional Neural Networks (CNN) and MobileNet to assess quality and detect defects. This project addresses the limitations of manual rice grading by providing a fast, accurate, and objective computer vision solution.

-Classes (11 Categories)

	Broken Rice
	Chalky
	Damaged Rice
	Discolored Rice
	Standard Rice
	Grade 1
	Grade 2
	Grade 3
	Grade 4
	Grade 5
	Premium Grade

-Sample Images of Rice Grain Classes
 researchgate.netlink.springer.comlink.springer.comfao.orgagriculturejournal.orgmdpi.com





Project Overview
	Manual rice grain classification is time-consuming, subjective, and prone to errors. This project leverages deep learning to automate the process, enabling faster and 		more accurate quality assessment for the agrotechnology industry.
Key Features:

	Multi-class classification (11 classes) using image processing and deep learning.
	Models: Custom CNN and Transfer Learning with MobileNet.
	Web application built with Flask for easy prediction on uploaded images.
Pre-processing:
	Grayscale conversion, binary thresholding, segmentation.
	Feature extraction: Color, morphological, and textural features.

Dataset: 
	Sourced from Kaggle (multi-class rice grain images).
	Note: Due to size constraints, the full dataset is not included in the repo. Download it from the original source or similar Kaggle datasets for rice quality  		 	 		classification.
	
Model Architectures
	Custom Convolutional Neural Network (CNN)
	A standard CNN architecture for feature extraction and classification.
	MobileNet (Transfer Learning)
	Lightweight and efficient model ideal for deployment on resource-constrained devices.
	researchgate.netresearchgate.net

Installation

	Clone the repository:Bashgit clone https://github.com/yourusername/rice-grain-classification.git
	cd rice-grain-classification
	Create a virtual environment (recommended):Bashpython -m venv venv
	source venv/bin/activate  # On Windows: venv\Scripts\activate
	Install dependencies:Bashpip install -r requirements.txtExample requirements.txt content:texttensorflow>=2.0
	keras
	opencv-python
	numpy
	flask
	pillow
	matplotlib

Usage
	Training the Model
	Run the training script (e.g., train.py or Jupyter notebook):
	Bashpython train.py

Data split: 
	90% training, 10% validation.

Running the Web App
	Launch the Flask application for predictions:
	Bashpython app.py
	
	Open http://127.0.0.1:5000 in your browser.
	Upload a rice grain image and select the model (CNN or MobileNet) to get the predicted class.

Example Prediction
	Upload an image → Model processes → Displays predicted grade (e.g., "Premium Grade" or "Chalky").
	Results

High accuracy achieved with both CNN and MobileNet.
MobileNet offers faster inference with comparable performance.
Evaluated on diverse images with varying intensity, position, and orientation.

Future Scope

	Integration with mobile apps for on-field quality checking.
	Expand to detect more defects or varieties.
	Real-time video processing for conveyor belt sorting.
	Deployment on edge devices.

Contributing
	Contributions are welcome! Please fork the repo, create a branch, and submit a pull request.
	License
	This project is licensed under the MIT License - see the LICENSE file for details.
	Acknowledgments

Inspired by research in computer vision for agriculture.
	Dataset and ideas from various Kaggle contributions and academic papers.
