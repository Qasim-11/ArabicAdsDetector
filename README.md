# Arabic Assignment Ads Detector

## Overview
This project is an **Arabic ads detector** designed to identify and filter out unwanted promotional messages in Arabic university WhatsApp groups or similar chat platforms. These messages typically offer illegal assignment, homework, or project solving services, which are disruptive and against academic ethics.

The detector analyzes incoming text messages and classifies them as either:

- **Ad-like message** (offering academic services such as assignment help, project completion, etc.)  
- **Non-ad message** (regular chat or legitimate content)

When an ad-like message is detected, the user sending it can be automatically removed or flagged to maintain the integrity and focus of the group.

---

## Features
- Detects Arabic text ads promoting assignment, homework, project, or medical excuse services.
- Utilizes a machine learning model trained on real-world positive (ads) and negative (non-ads) examples.
- Easily integratable into chat moderation bots or platforms like WhatsApp via APIs.
- Provides fast and accurate binary classification (`ad` / `not ad`).

---

## Dataset
The model is trained on a dataset of Arabic messages including:

- Positive examples: Various types of academic service ads offering illegal help.
- Negative examples: Normal chat, complaints, unrelated text, or non-ad messages.

---

## How It Works
1. The input text message is preprocessed and tokenized.
2. The trained model predicts whether the message is an ad.
3. If classified as an ad, moderation action (e.g., kicking the user) can be triggered.

---

## Installation

```bash
git clone https://github.com/yourusername/arabic-assignment-ads-detector.git
cd arabic-assignment-ads-detector
pip install -r requirements.txt
```
Then make an instance of the class `Model` and load the pretrained model. Boom, you have an AI detector, you can use it as simple as that.
Note that in the notebook, I wrote a function `predict` that takes a string text and output the prediction, you don't need to write your own prediction function.
