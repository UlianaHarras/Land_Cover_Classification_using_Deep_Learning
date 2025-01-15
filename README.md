# Land_Cover_Classification_using_Deep_Learning
Final project at WBS Coding School (Data Science Bootcamp)

**The project is aimed to classify satellite images (EuroSAT dataset) to 10 different land cover classes using Deep Learning model.** 
Land cover classification is categorizing the Earth's surface into predefined classes such as water, vegetation, urban areas, etc. using satellite/aerial imagery. 

The classes are the following:
* Annual Crop
* Forest
* Herbaceous Vegetation
* Highway
* Industrial
* Pasture
* Permanent Crop
* Residential
* River
* Sea/Lake

The **data** is pre-processed and already splitted to training, validation and test datasets. It contains 64x64 pixel RGB images collected from the Sentinel-2 satellite and can be found here: https://www.kaggle.com/datasets/apollo2506/eurosat-dataset/data  

The **tools** used in the project: Python libraries: Pandas, NumPy, Matplotlib, TensorFlow, Json, PIL.

The **approach** used is **Convolutional Neural Network (CNN)**, which is a type of deep learning model that is good at working with images. It’s designed to recognize patterns like shapes, textures, and objects in pictures. A CNN is:
1. Breaking the image into small parts.
2. Looking for simple patterns (e.g., edges or shapes).
3. Combining these patterns to identify the full object.

**Final_project_Land_Cover_Classification.ipynb** is a Google Colab notebook, containing: the code to load, preprocess and visualise images, several CNN models from the very simple one to the more complex one, the code to train, evaluate the model and analyse, which classes of images were misclassified. The model has an accuracy of **96%** on training data, and **92%** on test data. **model_cnn3_09_01_96-91-92.keras** is the file with the model.

The performance of the model has been compared to human performance. File **test_my_label.xlsx** or files **test_my_label - Stats.csv and  test_my_label- test_my_label.csv** include the test data and label(class) assigned by human. The accuracy of labeling test images by human is **90%**. Although accuracy is quite similar to the accuracy of the model, human was **324 times slower** labeling the images than the model. 

**Final_presentation_Uliana_Harras_2025_01_15.pptx** is a presentation for non-technical users.


