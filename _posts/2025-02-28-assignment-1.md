---
title: "Assignment 1: Working with a Corpus S25"
last_modified_at: 2025-02-19T22:00:00-05:00
categories:
  - Assignment
tags:
  - Working
---
# Title
This exercise has three main elements:
1. choosing a corpus of three texts (or three sets of texts) you would like to work with
2. using digital textual analysis tools to see what kind of exploratory data analysis (EDA) you can do using that corpus,
3. assembling the evidence in a piece of web-facing written work along with visuals.

**Due Date:** Thursday Feb 28, 2025 
{: .notice}

## Step 1: Three different sets of articles from a single class or multiple classes in your major.Permalink

Whatever your choice may be, you have the option of using three legitimate files, or substituting one of the files with a fake genAI created one, as we did in the case of the science fiction texts. Generating a text of equivalent length with genAI may take considerable extra effort.

Alternatively, you can source your text files from anywhere else, but if you make a custom corpus, please consult with the instructor before beginning this process. The texts can be short stories or articles, but not less than 1000-2000 words. If you choose your own files, include a copy of all three of them in your assets folder and create links to them for your readers to examine. If you are not working with texts from Project Gutenberg, then you will need to follow the instructions in the notebook for uploading your own files.

## Step 2 You should do some general research about the authors, the text, the contents. You will want to justify briefly the selection of texts in your assignment. You might even browse them briefly to know generally what they are about. This will help you to contextualize your findings. This is important so that you are not studying the corpus without a general idea of its contents.Permalink

> You want to choose texts which have something in common, but also can be thought about as different. The more you know about the texts, the more meaningful the “distant reading” will be.

## For this exercise you must use both (1) Voyant Tools and (2) the RMarkdown notebook in posit.cloud Identifying the Most Distinctive Words in Three (Sets of) Texts. The RMarkdown notebook in posit.cloud Summarizing a text from Project Gutenberg in a wordcloud is optional.

If you want to combine sets of texts from Project Gutenberg into one, you can do so by creating a list of ID numbers like this:

>gutenbergbook <- gutenberg_download(c(textID1, textID2, textID3, etc))

## Step 4: Build a set of screenshots from your exploratory analysis. Please be sure to include at least two (2) of them.Permalink

## Step 5: Use one iframe from Voyant Tools so that you have one interactive visualization. You can get an iframe from the export URL tab. It is called an html snippet. One example looks like this:Permalink

```
<iframe style='width: 444px; height: 408px;' src='https://voyant-tools.org/tool/Cirrus/?corpus=8d8c7ce89087801d676ff4f77d5391fc'></iframe>
```

## Find two (2) of the readings/resources from this term and include references to them in your essay. Feel free to refer to external resources.Permalink

Consider the questions raised in class on making Markdown posts legible: using Markdown Live Preview and Hemingway App as you compose your response. Keep the F-shape principle for web writing in mind too!

## Guiding Questions (you do not need to answer all these questions):

* What did you know about the subject before you began your analysis?
* What does computer-assisted analysis allow you to see that you wouldn’t have seen in a linear read? Would a linear read of all the texts have been possible in the time frame allotted?
* What is a trend you can identify in the materials? What are you able to learn by looking at the text the way you did?
* Were there any surprises in your exploration?
* If you reran the code or redid your Voyant Tools exploration did you get the same results every time? If not, why do you think?
* Are there any differences in the ways the different wordclouds visualize the words?
* How limiting (if at all) was the notebook that required you to compare three texts, i.e. to compare one text to two others? Was there something else you would like to do?
* How well would this assignment work for a language other than English? If you worked on texts not in English, what challenges did you face?

You assignment should be about 1500 words, or about a 8 minute read. Please publish it to your course site with a visible tab.