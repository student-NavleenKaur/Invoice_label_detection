Invoice Label Detection
This repository features a YOLOv8-based model for extracting key information from digital invoices. Trained on custom datasets, the model detects fields such as invoice numbers, dates, sellers, buyers, and totals, aiming to automate and streamline invoice data extraction.

Dataset
The dataset used for training and testing the model can be accessed via the following link:
[Open dataset](https://drive.google.com/drive/folders/1BmU_WXsHq7RA6jnAFzcrl61vnG-HRUx9?usp=drive_link)


Using the Dataset with Google Colab
Follow these instructions to use the dataset with the provided Google Colab notebook:

1. Open the Google Colab Notebook
Navigate to the [python file](Invoice_label_extraction.ipynb) present in this repository containing the code..

2. Mount Google Drive
In the Google Colab notebook, you need to mount your Google Drive to access the dataset.
 Run the following code cell:
```python
from google.colab import drive
drive.mount('/content/drive')
```

This will prompt you to authenticate and grant access to your Google Drive.

3. Set the Dataset Path
Once you have mounted Google Drive, set the path to your dataset folder in the notebook. Replace Your_Folder_Name with the actual name of the folder where you placed the dataset:
```python
dataset_path = '/content/drive/My Drive/Your_Folder_Name/'
 ```

4. Load and Explore the Dataset
Use the following code snippet to list files in the dataset directory and explore its contents:
```python
import os
 # List files in the dataset directory
dataset_files = os.listdir(dataset_path)
print(dataset_files)
 ```

5. Training the Model
Follow the instructions in the notebook to start training the YOLOv8 model. Ensure that the dataset is correctly referenced in the notebook's configuration.

6. Testing and Validation
After training, use the provided sections in the notebook to test and validate the model's performance. Follow the instructions to run inference on new invoice images.

Troubleshooting
Dataset Path Issues: Make sure that the dataset path in the notebook matches the folder structure in your Google Drive.
Mounting Errors: Verify that you have granted necessary permissions to Google Drive.
Model Training Issues: Check the Colab notebook for any error messages related to data loading or model training.
Contributing
If you have suggestions or improvements, please contribute by opening an issue or submitting a pull request.
