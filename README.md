# Emotion-Aware Mental Health Insight – Part 2: Text Sentiment Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-1.13-red)](https://pytorch.org/)
[![License](https://img.shields.io/badge/License-GPLv3-green)](https://www.gnu.org/licenses/gpl-3.0.en.html)

This repository contains the **Text Sentiment Analysis** module, the second core component of the **Emotion-Aware Mental Health Insight System**. It complements Part 1 (Speech Emotion Recognition) by analyzing user-generated text in online communities to predict emotional tone and identify mental health trends.

---

## Introduction

Part 2 implements the methods described in the paper:
*"Predicting User Emotional Tone in Mental Disorder Online Communities,"* published in Future Generation Computer Systems (FGCS).

This module leverages **VADER Sentiment Analysis** and a GRU-based RNN to extract sentiment features from Reddit posts and comments, predicting users’ emotional tone. When combined with Part 1 (speech emotion recognition), the full system can analyze both voice and text to provide cross-modal emotional insights.

---

## Dataset

The dataset contains posts and comments from four mental health-focused subreddits:

* r/Anxiety
* r/bipolar
* r/depression
* r/SuicideWatch

Statistics for each subreddit are included for detailed analysis.

---

## Repository Structure

* **REDDIT\_SCRAPPER:** Collects subreddit posts and comments via Reddit API.
* **PRE\_PROCESSING:** Prepares data with VADER sentiment scores and thread statistics.
* **PAPER\_RESULTS:** Trains the GRU model and performs result analysis.
* **REVIEW\_EXPERIMENTS:** Additional experiments, including confidence intervals and case studies.
* **src/**: Contains the core PyTorch model implementation and helper scripts.

This module is intended to work alongside **Part 1 (Speech Emotion Recognition)** for a complete emotion-aware system.

---

## Setup and Usage

1. Clone the repository and follow the provided directory structure.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. **Data Collection:** Run `REDDIT_SCRAPPER` notebook to fetch subreddit data.
4. **Data Preprocessing:** Run `PRE_PROCESSING` notebook or download preprocessed datasets.
5. **Model Training:**

   * Train from scratch on a GPU-enabled machine, or
   * Load pre-trained parameters to run the `PAPER_RESULTS` notebook in testing mode.

---

## Reproducing Results

After running the above steps, the trained model will:

* Generate a results table aligned with the paper’s findings.
* Provide case studies and visualizations of emotional trends in subreddit discussions.
* Integrate with Part 1 outputs for combined speech and text emotion insights.

---

## Future Development and Roadmap

* Implement a command-line interface for streamlined use.
* Expand the model to additional online communities.
* Integrate multimodal analysis combining voice and text for more accurate emotional detection.
* Develop dashboards for visualizing cross-modal emotional trends.

If you want, I can now create a **combined project README** that covers both Part 1 and Part 2 in a single professional homepage for GitHub. Do you want me to do that?
