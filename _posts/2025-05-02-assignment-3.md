---
title: "Assignment 3"
last_modified_at: 2025-02-19T22:00:00-05:00
categories:
  - Assignments
tags:
  - Working
---
## Introduction
*Written and researched by Lucas Lin.*

This report examines the capabilities of AI in recognizing and classifying attributes on AI-generated cat images sourced from CIVITAI. By analyzing how well AI models can identify predefined attributes such as Realistic, Artistic, Surreal, Humorous, and Abstract, we aim to assess the accuracy and reliability of these models in interpreting visual data. This study not only evaluates the technical performance of AI but also explores the broader implications of AI-driven image classification in the context of digital content creation.

## 1. Building the Corpus
### 1.1 Corpus Desciption
* **Source:** AI-generated images from CIVITAI, a platform for sharing and downloading AI models.
* **Number of Images:** 99
* **Number of Images with Prompt:** 67
* **Attributes:** Realistic, Artistic, Surreal, Humorous, Abstract
* **Organizaiton:** Images are organized into subfolders based on the attributes mentioned above.

### 1.2 Data Gathering
I used the extension IMAGE DOWNLOADED and downloaded 99 images that were recently uploaded to CIVITAI on May 1 within the section of cat-generated images. The filter used was the default one by week, which provided a representative sample of the most recent AI-generated cat images. This approach ensured that the dataset was current and relevant to the ongoing trends in AI-generated imagery.

### 1.3 Organizing Corpus
After downloading the images, I systematically searched for each image's prompts. Some images did not show their prompts, but for those that did, 67 of them, I collected their prompts and used KIMI to categorize them based on their prompts into equal amounts of subfolder categories. This process involved manually searching for each image's prompts and organizing them into corresponding attribute folders. It was a time-consuming task that required careful attention to detail, as I had to go back and edit the organization multiple times to ensure accuracy and consistency.

## 2 Clustering Ecercise (Organe Data Mining)
### 2.1 Different 
Using the provided images2.ows workflow, I tested clustering with Inceptionv3 and other algorithms to see how they organize the data. I explored the following questions:
How does one built-in algorithm such as Inceptionv3 in ODM cluster the data?
Do other algorithms give you different results?
What features seem to be most characteristic of the different quadrants of the image plot?
Using hierarchical clustering, isolate specific clusters to look more closely.
How “in reading a corpus of visual culture through a neural network, [are you] always also doing the reverse?” (Impett and Offert, 2024)

### 2.2 Analysisng the Results
Screenshot the main image plot;

Method explain how Isolate clusters via hierarchical clustering; annotate findings.

Reflect: How does the algorithm’s view differ from yours?
### 2.1 Comparison Insights
Compare algorithm outputs.

Address the Impett & Offert quote on neural networks.

## 3 Classification & Consfusion Matrix
### 3.1 Categorizing Images
Creating clssification system
### 3.2 Preditiong
What to expect 
Analysing any errors that occured and why
### 3.3 Reflection
Refine categories if needed.
How well did any of the built-in algorithms you chose predict the categories you established?
Did you go back and adjust any of your categories?
When you isolate the cases of “false positives”, i.e. mis-predictions, can you understand why the algorithm got them wrong? (Think about the Monet/Manet mis-prediction case we saw in class).
If you could train your own algorithm what would you aim to teach it?
Reference Distant Viewing (Arnold & Tilton).

## 4 Multimodal Analysis (CLIP/DV Explorer)
### 4.1 Generate Captions
Use 2DCLIP/DV Explorer to auto-caption images. Compare AI-generated text to my own interpretations.
### 4.2 Explore Language-Image Relationship
Try to decipher how CLIrganize the corpus. Revisit the Impett & Offert quote in this context.

## 5 Overall
### 5.1 Summary
Summarize findings from Parts 2–4.
### 5.2 Key Insights
### 5.3 Takeaway

## Links & Sources & Assets
### Links
### Sources
### Assets

**✅ Working**
<br/>
Due: May 11, 2025 23:59 PM
{: .notice}