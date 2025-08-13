# SentimentWell
A PyTorch implementation of a GRU-based RNN to predict users' emotional tone in online communities related to mental health.

Introduction
This repository contains the code for the paper "Predicting User Emotional Tone in Mental Disorder Online Communities", published in the Future Generation Computer Systems (FGCS) journal's special issue on sentiment analysis systems. The model leverages the VADER Sentiment Analysis tool to extract sentiment features from Reddit posts and comments.

About the Dataset
The study uses a dataset of posts and comments from four mental health-focused subreddits: r/Anxiety, r/bipolar, r/depression, and r/SuicideWatch. The dataset statistics for each subreddit are provided for further analysis.

Contents and Usage
This repository includes four main Python notebooks, each designed for a specific part of the workflow, allowing users to reproduce the paper's results:

REDDIT_SCRAPPER: Collects data from subreddits using Reddit's API.
PRE_PROCESSING: Prepares data for training by consolidating VADER sentiment scores and key thread statistics.
PAPER_RESULTS: Trains the model and performs result analysis.
REVIEW_EXPERIMENTS: Conducts additional confidence interval experiments and other analyses.
The src folder contains essential Python files, including the main PyTorch model implementation.

Setup and Usage
To get started:

Follow the provided directory structure to organize files correctly.
Install dependencies with pip install -r requirements.txt.
To replicate the paper's results, follow these steps:
Data Collection: Run the REDDIT_SCRAPPER notebook locally to download subreddit data.
Data Preprocessing: Run the PRE_PROCESSING notebook (recommended on Colab for TPU support), or download the preprocessed dataset.
Model Training: Choose between training the model from scratch on a GPU-enabled machine or loading pre-trained parameters to run the PAPER_RESULTS notebook in testing mode.
Reproducing Results
The pipeline aims for easy reproducibility of the original results. After completing these steps, the trained model will generate a results table and provide case studies on specific threads.

Future Development & Support
A command-line version of the model is planned for streamlined use. For questions or suggestions, contact the authors by email.

License & Disclaimer
This research code is licensed under the GNU General Public License Version 3 (GPLv3) and is provided without any warranty for specific use.

Authors: Bárbara Silveira, Henrique S. A. Silva, Fabricio Murai, Ana Paula C. da Silva

Citation: Use the provided BibTeX entry to cite this paper if using or referring to the research in other work. The study explores how Reddit interactions in mental health communities affect users' emotional states and presents a model that predicts emotional tone changes based on these interactions. The results suggest that social support on these platforms can positively impact users' emotional well-being.
