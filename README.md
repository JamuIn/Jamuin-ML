# Jamuin-ML
# Introduction
<p align='center'>Team ID:C23-PS445 </p><br>

## Our Machine Learning Team
- Dian Alhusari (M151DSX1521) - Universitas Brawijaya [Github](https://github.com/alhusari2)
- Yohanes Egi Pratama Yudoutomo (M356DKX4808) - Universitas Teknokrat Indonesia [Github](https://github.com/hanesegi)

# Model Description:
a machine learning model was created to classify images of herbal ingredients that we often encounter to be recommended into herbal products, including:

## Built with
- [Python](https://www.python.org/ "Python")
- [TensorFlow](https://www.tensorflow.org/ "TensorFlow")
- [Flask](https://flask.palletsprojects.com/en/2.1.x/ "Flask")
- [Google Cloud Run](https://cloud.google.com/run)
- [Google Colab](https://colab.research.google.com/ "Google Colab")

# Dataset:
dataset of herbal ingredients obtained by scraping, and manually [data](https://drive.google.com/drive/folders/1KDyy5kXO6M25G-KQ7x3pyj171u4ZTk81?usp=drive_link)
<p>Preview of the image and data used are shown in the picture below:</p>
<h5>Kunyit</h5>
<img src="https://github.com/JamuIn/Jamuin-ML/blob/main/Dataset/assetdata.PNG?raw=true"
     title="Kunyit">
     
# Arsitektur Model
Arsitektur Model
<center><img src="Model/arsitektur.png"></center>

# Make RESTfull API with Flask and Cloud Run
1. Prepare prediction model in "h.5" format, file are stored in "ML-Backend" folder 
2. Write main.py base on machine learning testing model, files are saved in the "ML-Backend" folder
3. Create file named "requirement.txt" for library you need for running our code
4. Create file named "Dockerfile" for run system in our container
5. Create file named ".dockerignore" for ignore system to ignore spesific file.
6. Create folder static/uploads to save photos for prediction progress.
7. Create new Project in Google Cloud
8. Active Cloud Run API and Cloud Build API
9. Install and init Google Cloud SDK (U can Use this link : https://cloud.google.com/sdk/docs/install)
10. Use Cloud Build to import our code to our cloud services (gcloud builds submit --tag gcr.io/<project_id>/<function_name>)
11. Use Cloud Run to deploy our API (gcloud run deploy --image gcr.io/<project_id>/<function_name> --platform managed)
