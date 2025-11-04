# Object-Detection-Using-YOLOv3
YOLOv3 Obejct Detection Project
Project Description
This project is based on YOLOv3, running target detection tasks on COCO dataset and customized dataset. Experiments are conducted to demonstrate the impact of preprocessing on the performance of target detection, and the model performance is evaluated on multiple metrics, including mAP, Accuracy, Recall, and F1 score.

Running Environment
Platform: Google Colab
Tools & Dependencies:
YOLOv3: AlexeyAB/darknet
Data annotation tool: Labelme

Workflow
Step 1: Environment Configuration
Install required libraries: Execute code in Google Colab to install dependencies.
Download YOLOv3 weights and COCO dataset: Clone the code base from AlexeyAB/darknet and download the weights file. Download the COCO dataset and unzip it.
Validate YOLOv3 pre-training model operation: randomly select 10 images in the validation subset of the COCO dataset for testing. Run the model to generate a prediction JSON file.

Step 2: Evaluate the performance of the COCO dataset
Performance metrics: Evaluate the prediction results of the COCO dataset and calculate the following metrics:
Mean Accuracy (mAP)
Accuracy
Recall
F1 Score
Confusion Matrix

Step 3: Upload customized dataset
Label the data:
Label the custom dataset using Labelme and generate an annotation file.
Convert the Labelme format annotation file to COCO format.
Upload dataset (create necessary folders):
Create own_dataset and upload custom dataset image.
Create own_dataset_gt and upload the Ground Truth JSON file for the custom dataset.

Step 4: Preprocess the custom dataset
Data preprocessing:
Perform image resizing and data enhancement (e.g., rotation, cropping, etc.) on the custom dataset.
Create processed_own_dataset to save the pre-processed images.
Comparison of effects:
Create output_own_image to save two images for comparing the effect of preprocessed and unpreprocessed.

Step 5: Run custom dataset target detection
Execute YOLOv3 detection:
Run the YOLOv3 model on the preprocessed custom dataset.
Generate a prediction JSON file.
Compare results:
Repeat the detection process on an unprepared dataset.
Evaluate custom dataset performance:
Evaluate the detection results and calculate mAP, Accuracy, Recall, and F1 scores.

Output Files
Prediction file:
The prediction.json file containing bounding box and classification information for model detection.
Results folder:
own_dataset: uploaded image of the custom dataset.
own_dataset_gt: Ground Truth JSON file for the custom dataset.
processed_own_dataset: pre-processed image.
output_own_image: two images for comparing preprocessed and unpreprocessed images.
Evaluation Report:
Contains the evaluation results of the performance metrics for each dataset.

Colab Instructions
Open the Colab Notebook file for your project.
Execute the code units in order to complete the following tasks:
Environment Configuration.
Data set upload and preprocessing.
Model run and evaluation.
Download the generated results file for local analysis.

