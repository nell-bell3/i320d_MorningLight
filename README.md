Spotify Churn Project

This repo has all the code and files from our final project on predicting Spotify user churn. Everything is split into separate notebooks so it's easy to follow what each part does.

Notebooks

1. beat_the_churn_oldandnew_EDA.ipynb
This notebook has all the exploratory data analysis. It’s where we look at trends in the dataset, check distributions, clean the data, and basically figure out what we’re working with.
- Includes: Basic EDA, Automated EDA using ProfileReport, and Advanced EDA techniques

3. Churn_LR.ipynb
This notebook has the full linear regression / model-training code. When you run it, it will download and save the trained model file that the dashboard uses.

4. ChurnDashboard.ipynb
This notebook has the code for the Streamlit dashboard. It uses the model generated from Churn_LR.ipynb.

5. Churn_EDA.ipynb (Deprecated)
This notebook has the original exploratory analysis done on the first dataset, beat_the_churn_oldandnew_EDA.ipynb includes full range EDA on both the old and new datasets. 

Datasets

Spotify_Churn_32000.csv
This is the main dataset used for everything now. You need this file downloaded in the same directory when running any of the notebooks.

Spotify_Churn_Dataset.csv
This was the original dataset with ~8,000 rows. We kept it in the repo, but the newer 32,000-row dataset replaced it for training and evaluation.

Running the Dashboard

After you run the Churn_LR.ipynb notebook and the model file is created, you can launch the dashboard by running:

streamlit run app.py


This will open the interactive churn predictor dashboard in your browser.
