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
* **Attributes:** Realistic, Artistic, Surreal, Humorous, Abstract (Attributes are given to only images with prompts)
* **Organizaiton:** Images are organized into subfolders based on the attributes mentioned above.

### 1.2 Data Gathering
How I did is by using the extension IMAGE DOWNLOADED and downloaded 99 images from the CIVITAI website on the most recent upload on May 1, 2025 within the section of cat-generated images. The filter used was the default one by week, which provided a representative sample of the most recent AI-generated cat images of that week. This approach ensured that the dataset was current and relevant to the ongoing trends in AI-generated imagery.

After downloading the images, I went back to each image individually to look for their prompt. I recorded each prompt for the images that had them, which was essential for the categorization process.

### 1.3 Organizing Corpus
To ensure a balanced and meaningful analysis, I decided to categorize the images into five distinct categories: Realistic, Artistic, Surreal, Humorous, and Abstract. Each category was chosen to reflect different styles and themes commonly found in AI-generated cat images. I found these categories by giving KIMI all the prompts of the images and having it categorize finding a common ground. I asked for multiple sets of categories and chose the following one. I then categorized based on the results the AI gave me as I wanted to both follow the mindset of the AI and also be more reliant on the prompt and how the AI thinks rather than I decide based on feeling. Here's the rationale behind each category:

1. **Realistic and Photorealistic**: This category includes images that aim to depict cats in a highly detailed and lifelike manner, often with photorealistic qualities. These images typically feature natural settings, detailed textures, and accurate anatomical representations.

2. **Artistic and Illustrative**: This category encompasses images that exhibit artistic styles, such as painterly, impressionistic, or illustrative techniques. These images often include elements like abstract backgrounds, stylized features, and a focus on artistic expression.

3. **Surreal and Fantasy**: This category features images that incorporate surreal or fantastical elements, such as exaggerated features, dreamlike settings, or otherworldly themes. These images often push the boundaries of reality and imagination.

4. **Humorous and Meme-like**: This category includes images that are designed to be humorous or meme-like, often featuring playful or exaggerated scenarios. These images are intended to evoke laughter or amusement and may include text or other elements that enhance their comedic effect.

5. **Abstract and Minimalist**: This category contains images that are characterized by abstract or minimalist design principles. These images may feature simplified forms, geometric shapes, or a focus on color and composition rather than detailed representation.

To ensure that the categorization process was unbiased and focused solely on the prompts rather than the visual content of the images, I utilized KIMI to categorize the images based on their prompts. This approach helped to minimize any potential biases that might arise from subjective interpretation of the visual data. Since I more focused on the comparison of the prompt and the image itself if the algorithm is able to recognize. I should categorize based on the prompt rather than the image itself.

## 2 Clustering Exercise (Organe Data Mining)
### 2.1 Different 
I began clustering the images without their categories in mind just to see if I could decipher how the algorithm was categorizing the images. This approach aligns with the concept that "in reading a corpus of visual culture through a neural network, [are you] always also doing the reverse?" (Impett and Offert, 2024). By analyzing how AI interprets visual data, we gain insights into the AI's own categorization logic and biases.

The below are screenshots of the different clustering results and how I try to identify how each algorithm clusters them.

| Cluster Screenshot | Algorithm |
|-------------------|-----------|
| ![This is Cluster Guess 0](/assets/images/assignment-3/ClusterGuess0.png)| Inceptionv3|
| ![This is Cluster Guess 1](/assets/images/assignment-3/ClusterGuess1.png)| SqueezeNet|
| ![This is Cluster Guess 2](/assets/images/assignment-3/ClusterGuess2.png)| Painters |
| ![This is Cluster Guess3](/assets/images/assignment-3/ClusterGuess3.png)| DeepLoc |

What I noticed is that ODM clustering algorithms do organize the data differently. Inceptionv3 focuses more on similar objects, for instance if they both showcase a black cat. SqueezeNet is more about its thematic. DeepLoc is more by its color brightness, with the darker ones on the top left and bright ones bottom right. Painters is a by color and type.

This observation aligns with Impett and Offert's concept, as it demonstrates how AI algorithms interpret visual data in ways that might differ from human perception. Each algorithm brings its own biases and methods to the task, which can lead to different clustering outcomes. By examining these outcomes, we can infer how AI 'reads' visual culture and how it might 'write back' its understanding into new categorizations or interpretations.

## 3 Classification & Consfusion Matrix
### 3.1 Categorizing Images
As mentioned before, creating a classification system based on the attributes: Realistic, Artistic, Surreal, Humorous, Abstract. I found these categories by giving KIMI all the prompts of the images and having it categorize finding a common ground. I asked for multiple sets of categories and chose the above one. 
### 3.2 Predition
What i expect is for some of the classification to be accurately identified given they are image generated based on the classified wording.
However the resulting did not meet what i was expecting as it was all over the place for it to clearly identify some categories.
|||
|--|--|
|![This is Hierchy 1](/assets/images/assignment-3/Hierchy1.png)||
|Inceptionv3||
|||
|||

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