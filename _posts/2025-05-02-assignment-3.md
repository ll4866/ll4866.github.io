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

This assignment examines the capabilities of AI in recognizing and classifying attributes on AI-generated cat images sourced from CIVITAI. By analyzing how well AI models can identify predefined attributes such as Realistic, Artistic, Surreal, Humorous, and Abstract, we aim to assess the accuracy and reliability of these models in interpreting visual data. This not only evaluates the technical performance of AI but also explores the broader implications of AI-driven image classification in the context of digital content creation.

## 1. Building the Corpus
### 1.1 Corpus Desciption
* **Source:** AI-generated images from CIVITAI, a platform for sharing and downloading AI models.
* **Number of Images:** 99
* **Number of Images with Prompt:** 67
* **Attributes:** Realistic, Artistic, Surreal, Humorous, Abstract
* **Organizaiton:** Images are organized into subfolders based on the attributes mentioned above.

### 1.2 Data Gathering
I used the extension IMAGE DOWNLOADED and downloaded 99 images that were recently uploaded to CIVITAI on May 1, 2025 within the section of cat-generated images. The filter used was the default one by week, which provided a representative sample of the most recent AI-generated cat images. This approach ensured that the dataset was current and relevant to the ongoing trends in AI-generated imagery.

### 1.3 Organizing Corpus
To ensure a balanced and meaningful analysis, I decided to categorize the images into five distinct categories: Realistic, Artistic, Surreal, Humorous, and Abstract. Each category was chosen to reflect different styles and themes commonly found in AI-generated cat images. Here's the rationale behind each category:

1. **Realistic and Photorealistic**: This category includes images that aim to depict cats in a highly detailed and lifelike manner, often with photorealistic qualities. These images typically feature natural settings, detailed textures, and accurate anatomical representations.

2. **Artistic and Illustrative**: This category encompasses images that exhibit artistic styles, such as painterly, impressionistic, or illustrative techniques. These images often include elements like abstract backgrounds, stylized features, and a focus on artistic expression.

3. **Surreal and Fantasy**: This category features images that incorporate surreal or fantastical elements, such as exaggerated features, dreamlike settings, or otherworldly themes. These images often push the boundaries of reality and imagination.

4. **Humorous and Meme-like**: This category includes images that are designed to be humorous or meme-like, often featuring playful or exaggerated scenarios. These images are intended to evoke laughter or amusement and may include text or other elements that enhance their comedic effect.

5. **Abstract and Minimalist**: This category contains images that are characterized by abstract or minimalist design principles. These images may feature simplified forms, geometric shapes, or a focus on color and composition rather than detailed representation.

To ensure that the categorization process was unbiased and focused solely on the prompts rather than the visual content of the images, I utilized KIMI to categorize the images based on their prompts. By doing so, I aimed to create a diverse and representative dataset that would allow for a comprehensive analysis of the AI models' performance across different styles and themes. This approach helped to minimize any potential biases that might arise from subjective interpretation of the visual data.

## 2 Clustering Ecercise (Organe Data Mining)
![This is Orange Image Grid](/assets/images/assignment-3/Screenshot 2025-05-11 at 15.12.54.png)

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