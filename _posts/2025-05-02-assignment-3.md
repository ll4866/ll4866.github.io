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
To gather the data, I used the IMAGE DOWNLOADER extension to download 99 images from the CIVITAI website. These images were the most recently uploaded on May 1, 2025, within the section of cat-generated images. The filter used was the default one by week, which provided a representative sample of the most recent AI-generated cat images of that week. This approach ensured that the dataset was current and relevant to the ongoing trends in AI-generated imagery.
After downloading the images, I went back to each image individually to look for their prompt. I recorded each prompt for the images that had them, which was essential for the categorization process.

### 1.3 Organizing Corpus
To ensure a balanced and meaningful analysis, I decided to categorize the images into five distinct categories: Realistic, Artistic, Surreal, Humorous, and Abstract. Each category was chosen to reflect different styles and themes commonly found in AI-generated cat images. I found these categories by giving KIMI all the prompts of the images and having it categorize them, finding a common ground. I asked for multiple sets of categories and chose the following one. I then categorized based on the results the AI gave me, as I wanted to follow the mindset of the AI and be more reliant on the prompt and how the AI thinks rather than deciding based on my own feelings. Here's the rationale behind each category:

1. **Realistic and Photorealistic**: This category includes images that aim to depict cats in a highly detailed and lifelike manner, often with photorealistic qualities. These images typically feature natural settings, detailed textures, and accurate anatomical representations.

2. **Artistic and Illustrative**: This category encompasses images that exhibit artistic styles, such as painterly, impressionistic, or illustrative techniques. These images often include elements like abstract backgrounds, stylized features, and a focus on artistic expression.

3. **Surreal and Fantasy**: This category features images that incorporate surreal or fantastical elements, such as exaggerated features, dreamlike settings, or otherworldly themes. These images often push the boundaries of reality and imagination.

4. **Humorous and Meme-like**: This category includes images that are designed to be humorous or meme-like, often featuring playful or exaggerated scenarios. These images are intended to evoke laughter or amusement and may include text or other elements that enhance their comedic effect.

5. **Abstract and Minimalist**: This category contains images that are characterized by abstract or minimalist design principles. These images may feature simplified forms, geometric shapes, or a focus on color and composition rather than detailed representation.

To ensure that the categorization process was unbiased and focused solely on the prompts rather than the visual content of the images, I utilized KIMI to categorize the images based on their prompts. This approach helped to minimize any potential biases that might arise from subjective interpretation of the visual data. Since I more focused on the comparison of the prompt and the image itself if the algorithm is able to recognize. I should categorize based on the prompt rather than the image itself.

## 2 Clustering Exercise (Organe Data Mining)
### 2.1 Different Algorithms Clustering
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
As previously mentioned, I developed a classification system based on the attributes: Realistic, Artistic, Surreal, Humorous, and Abstract. These categories were determined by analyzing the prompts of the images with the assistance of KIMI.

### 3.2 Predition
I anticipated that the AI would accurately identify some classifications, given that the images were generated based on specific descriptive wording. However, the results did not fully meet my expectations, as the AI's classifications were inconsistent and did not clearly identify some categories.

### 3.4 Result
|**A. Inceptionv3**||
|--|--|
|![This is Hierchy 1](/assets/images/assignment-3/Hierchy0.png)||
|![This is Issue 1](/assets/images/assignment-3/Issue0.png)|Inceptionv3 was somewhat able to cluster the playful and serious images apart but it was not able to classify the categories I have established.|
|![This is Evidence 1](/assets/images/assignment-3/Evidence0.1.png)| C1. Most Surreal Fantasy but it seems that it attempted to categorize by how solid the color or texture is in this cluste| 
|![This is Evidence 2](/assets/images/assignment-3/Evidence0.2.png)| C2. Artistic illustrative is the most in this cluster but what the algorithm did was cluster the more animalistic playful images in this cluster | 
|![This is Results 0](/assets/images/assignment-3/Results0.png) | |


|**B. SqueezeNet**||
|--|--|
|![This is Hierchy 1](/assets/images/assignment-3/Hierchy1.png)|![This is Issue 1](/assets/images/assignment-3/Issue1.png)|
|![This is Evidence 1](/assets/images/assignment-3/Evidence1.1.png)| C3. It was successfully in picking out the drawing or manga-like cat images but given the prompts of these images were supposed to categorize them as Realistic. I guess in this definition of realistic is to make it look more authentic and human-made as possible rather than real existing.| 
|![This is Evidence 2](/assets/images/assignment-3/Evidence1.2.png)| C1. This section the algorithm was able to capture a sense of cinematic lighting and color of the images but it was not able to realize that it was fake and some parts were not realistic so it approached differently but close in identifying real.|
|![This is Evidence 2](/assets/images/assignment-3/Evidence1.3.png)| C2. Artistic - most of the images are supposed to be classified this way, and it does accomplish that as we can see that the algorithm senses artistic type. In this category, it is mostly the cats' faces, but the detail of the hair and eyes are so vivid and also portrayed as a self-portrait | 

SqueezeNet perfectly picked out the images by common traits and thematic sense.

These results indicate that while the algorithms were able to identify certain common traits and themes, they did not consistently classify the images according to the established categories. This suggests that the AI models may require further refinement to accurately interpret and categorize visual data based on textual prompts.

### 3.4 Reflection
Upon reviewing the classification results, several insights emerged:

- **Algorithm Performance**: The performance of the algorithms varied significantly. While SqueezeNet showed a strong ability to identify thematic elements and common traits, Inceptionv3 struggled with accurate categorization based on the predefined attributes.
- **Misclassification Accuracy**: The AI's ability to accurately classify images into the established categories was inconsistent. Some images could be considered for multiple categories but were placed in one due to the AI's interpretation. 

|For instance, consider the image|Prompt:|
|---|---|
| ![This is Image 66](/assets/images/assignment-3/IMAGE66.jpeg) | raw analog candid grainy photo 3 cute fluffy kitten/spider hybrids with fluffy spider legs (no paws), ultra high definition, on a cosy room bed, sunny morning light, we can see a human hand like a pov from the bed, one of the hybrids is climbing on the hand while other climb the bed, its a pov from me waking up so we can see the raw form of the body under the blanket, the room seems to be of a goth teem from the 90's|

The AI might label an image with a fantasy prompt as "realistic" because it looks closely at details like lighting, texture, and setting that make the image seem real. Even if the content is imaginary, if it looks like it could be real, the AI might put it in the realistic category. When categorizing the images, the AI uses the text of the prompts to decide where to place each image. It looks at the words and phrases in the prompts to understand the intended theme or style of the image. So, if the prompt describes an image with realistic qualities, the AI will categorize it as "realistic".

On the other hand, clustering is a different process where an algorithm groups images based on what it sees in the images themselves, not the prompts. The algorithm examines visual elements like color, shape, texture, and composition. If the algorithm detects patterns or features in the images that it associates with realism, it might cluster them together, even if the original prompt was fantastical.

The issue is the difference between words and imagery. This analysis, combined with insights from Distant Viewing (Arnold & Tilton), suggests that while AI has made significant progress in image classification, there is still room for improvement, particularly in how AI interprets and categorizes visual data based on textual descriptions.

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