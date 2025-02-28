---
title: "Assignment 1: Working with a Corpus S25"
last_modified_at: 2025-02-19T22:00:00-05:00
categories:
  - Assignment
tags:
  - Working
---
# Did Sherlock Holmes Influence Arthur Conan Doyle’s Later Works?

## Background Information  

We conducted a distant reading of Sir Arthur Conan Doyle’s works to examine whether the Sherlock Holmes series influenced his later books. Best known for creating the legendary detective, Doyle was a 19th-century British writer whose background in medicine shaped his storytelling, particularly in the forensic detail and logical reasoning found in his detective fiction.

In this assignment, we are curious to see whether writing the Sherlock Holmes series influenced Doyle’s later works. In particular, we ask whether Sherlock Holmes influenced Doyle’s writing afterward. If so, many of the words, themes, and stylistic choices from Sherlock Holmes would be carried over into his later books.

To explore this, we will conduct ‘distant reading’, gatherings and processing content, such as subjects, themes, persons, or places from a large number of textual items without engaging in the reading of the actual text (Drucker 113). The tools that we employ are `Voyant Tools` and `Posit.cloud (RMarkdown)`, which we will discuss in the following.

We gathered nine different books in the same genre—mystery—but written in different periods. Three books were selected from before Sherlock Holmes (*pre-SH*), three from the Sherlock Holmes series (*SHB*), and three from after Holmes (*post-SH*).  

## Hypothesis: The Sherlock Holmes Influence  
We hypothesize that writing the Sherlock Holmes series influenced Doyle’s later works. If so, his post-SH books should share notable similarities with the Holmes stories in vocabulary, themes, or narrative style. Given the overwhelming popularity of Holmes, it is possible that Doyle’s detective fiction left a lasting imprint on his writing, even beyond the mystery genre.

To test this, we used `Voyant Tools` and `Posit.cloud (RMarkdown)` for distant reading analysis, tracking word frequency, thematic patterns, and term repetition across the three time periods. By identifying linguistic and structural consistencies, we aimed to determine whether Doyle’s later works retained the influence of Sherlock Holmes or marked a departure from his detective fiction legacy.  

## Material Selection & Corpus  
All selected books were chosen based on their time of publication and genre, with a focus on mystery. While Arthur Conan Doyle continued to write mystery and detective fiction beyond the Sherlock Holmes series, our analysis focuses on the following works to examine stylistic and thematic shifts across different periods of his career. The pre-Sherlock Holmes books (The Gully of Bluemansdyke, The Captain of the Polestar, and My Friend the Murderer) explore themes of crime, supernatural elements, and human nature. The Sherlock Holmes books (A Study in Scarlet, The Sign of the Four, and The Adventures of Sherlock Holmes) serve as a benchmark for detective fiction, highlighting Doyle’s approach to logical reasoning and investigative storytelling. The post-Sherlock Holmes books (The White Company, Uncle Bernac, and Rodney Stone) shift towards war, politics, and historical narratives, marking a departure from detective fiction.

All materials were sourced from Project Gutenberg and categorized into three corpora:

| Category | Book Title & Description | Theme | Book Number |
|----------|--------------------------|-------|-------------|
| **Pre-Sherlock Holmes (pre-SH)** | [The Gully of Bluemansdyke (1881)](https://www.gutenberg.org/ebooks/40848) - A collection of short stories exploring crime, morality, and human nature, often with dark or tragic themes. | Mystery, Crime, Supernatural, Human Condition | #40848 |
|  | [The Captain of the Polestar and Other Tales (1883-1887)](https://www.gutenberg.org/ebooks/294) - A mix of supernatural and adventure stories, featuring ghostly encounters and mysterious events. | Mystery, Supernatural, Adventure | #294 |
|  | [My Friend the Murderer](https://www.gutenberg.org/ebooks/69260) (Late 19th c.) - A short story centered on crime and redemption, exploring themes of justice and guilt. | Mystery, Crime, Human Condition | #69260 |
| **Sherlock Holmes Books (SHB)** | [A Study in Scarlet (1887)](https://www.gutenberg.org/ebooks/244) - The first Sherlock Holmes novel, introducing Holmes and Watson as they solve a murder linked to past events in America. | Mystery, Detective | #244 |
|  | [The Sign of the Four (1890)](https://www.gutenberg.org/ebooks/2097) - A mystery involving a hidden treasure, betrayal, and an elaborate revenge plot. | Mystery, Detective | #2097 |
|  | [Adventures of Sherlock Holmes (1892)](https://www.gutenberg.org/ebooks/1661) - A collection of short stories showcasing Holmes’ detective skills through various intriguing cases. | Mystery, Detective | #1661 |
| **Post-Sherlock Holmes (post-SH)** | [The White Company (1891)](https://www.gutenberg.org/ebooks/903) - A historical adventure novel set during the Hundred Years’ War, following a group of English archers. | Historical, War | #903 |
|  | [Uncle Bernac (1897)](https://www.gutenberg.org/ebooks/10581) - A Napoleonic-era novel focused on espionage, war, and political intrigue. | Mystery, War (Napoleonic) | #10581 |
|  | [Rodney Stone (1896)](https://www.gutenberg.org/ebooks/5148) - A historical novel blending themes of boxing, aristocracy, and naval warfare in 18th-century England. | Historical, Boxing | #5148 |

*We refer to the bibliography [here](https://en.wikipedia.org/wiki/Arthur_Conan_Doyle_bibliography). The books analyzed in this study were sourced from Project Gutenberg, with their respective eBook ID numbers available for reference.*
{: .notice}

## Our Process  
A digital humanities workflow is composed of materials, processing, and visualization (Drucker 2). Our process involves selecting books from a large collection of Doyle’s works (Materials), inputting them into `Voyant Tools` and `Posit.cloud (RMarkdown)` to be examined (Processing), and then displaying them as graphs in posts within a blog form (Visualization).

We organized the selected books into three **corpora** based on their publication period:

1. **Pre-Sherlock Holmes (pre-SH):** Works written before the introduction of Sherlock Holmes, reflecting Doyle’s early style and themes.
2. **Sherlock Holmes Books (SHB):** Novels and short stories from the Holmes series, serving as a benchmark for Doyle’s detective fiction.
3. **Post-Sherlock Holmes (post-SH):** Works written after Holmes, where we examine whether elements of detective fiction persist or if Doyle’s writing shifts towards new themes.

To analyze linguistic patterns, thematic shifts, and word frequency distributions, we used two primary tools:

1. **Voyant Tools:** We combined all books within the same category into a single text file, creating three full-text documents—one for pre-SH, one for SHB, and one for post-SH. These combined text files were then uploaded into Voyant Tools, where we conducted word cloud analysis, frequency distributions, and general textual analysis to visualize recurring terms and themes across the different time periods.
2. **Posit.cloud (RStudio, ggplot2):** Used for in-depth statistical analysis, including graphical representations of recurring terms. Specific analyses included:
  * Identifying the Most Distinctive Words in Three (Sets of) Texts Compared vocabulary differences between pre-SH, SHB, and post-SH books.
  * Summarizing a text from Project Gutenberg in a word cloud - Generated visual representations of each corpus to highlight dominant themes.

This method follows the ideas discussed in Rockwell and Sinclair’s "The Measured Words: How Computers Analyze Text", which explains how computational tools process text by recognizing patterns rather than interpreting meaning (Rockwell & Sinclair, 25-43). While these tools helped us discover trends and explore Doyle’s writing, we combined them with human interpretation to ensure a more precise and meaningful analysis. Digital tools allowed us to identify shifts in word usage and themes, but human insight was essential to fully understand how Doyle’s style evolved and whether the influence of Sherlock Holmes persisted in his later works.

## RMarkdown (Posit.cloud) Results
### Word Cloud Results:

| Image | Image |
| This image is a word cloud from a corpus of all pre-Sherlock Holmes Books. | This image is a word cloud from a corpus of all pre-Sherlock Holmes Books. |
| | |
| This image is a word cloud from the selected novels post-Sherlock Holmes series. | |

### GGPlot Results
This time, we are using ggplot to reveal some more insights. The graph below shows the most recurring words in all selected Sherlock Holmes books. Based on the word cloud we generated previously, we expect the word ‘Holmes’ to appear at the top. In this scenario, we sorted out the words so that only words that reoccur above 150 times would show up.

image

#### First Iteration
image

#### Second Iteration
In this graph, we modified the values of the jitter size, height, and width. We also adjusted the colors so that it differs from the first iteration. We observed that the change allowed for more distinct words to show up.

image

#### Third Iteration
We decided to change things around this time by comparing pre-Sherlock Holmes books with the post and Sherlock Holmes series itself. The ggplot values are the same as the previous graph. Only the color is changed this time around. 

image

## Voyant Tools Results
### General
image

The table of basic information shows that Doyle wrote more extensively after Sherlock Holmes, with post-SH books having the highest word count. The Sherlock Holmes books have the shortest sentences (15.8 words per sentence), reflecting a concise and fast-paced style suited for detective fiction. In contrast, post-SH books have the longest sentences (19.9 words per sentence), suggesting a shift toward more complex and descriptive storytelling. Despite these changes, the 6% type-to-word ratio remains consistent, meaning Doyle’s vocabulary range stayed stable across all periods. However, the data does not clearly show that post-Holmes books retained the stylistic influence of Sherlock Holmes, suggesting that Doyle eventually moved toward a different narrative approach in his later works.

<iframe style='width: 1112px; height: 673px;' src='https://voyant-tools.org/tool/ScatterPlot/?docId=81a2da64a1c005e22b2471173ef02741&docId=2749a81ed25292d87f0d823a8029fb76&docId=5ebae079c45f874a11df3273e9852b7a&limit=206&dimensions=2&label=docs&label=summary&view=topics&corpus=1d58c9ad21987f6fbb38a73090d4017c'></iframe>

The scatter plot highlights a clear pattern in Doyle’s evolving writing style across different phases of his career. The close clustering of the Sherlock Holmes books (green) and the Pre-SH books (pink) suggests that while the detective stories had a distinct narrative focus, they still retained stylistic similarities with Doyle’s earlier works. This could indicate that his writing tendencies, such as sentence structure, word choice, or narrative flow, remained consistent even as he introduced the detective genre’s unique elements.

However, the Post-SH books (blue) are positioned farther away from the Sherlock Holmes books, suggesting a notable departure in style. This shift implies that Doyle did not continue the detective-driven approach in his later works but instead moved toward a different literary direction. Interestingly, the Post-SH books are still closer to the Pre-SH books than to the Sherlock Holmes books, reinforcing the idea that Doyle returned to his original writing style rather than carrying forward the characteristics of his most famous detective stories.

Despite this shift, the Post-SH books align with the Sherlock Holmes books along the Y-axis, which may suggest some lingering stylistic influences, such as sentence complexity or thematic elements. Overall, the scatter plot supports the interpretation that while the Sherlock Holmes stories represented a distinct and innovative phase in Doyle’s career, they did not permanently alter his broader writing tendencies. Instead, he eventually gravitated back toward his earlier narrative approach after concluding the Holmes series.

### Word Cloud Analysis

| <iframe style='width: 1112px; height: 673px;' src='https://voyant-tools.org/tool/Cirrus/?visible=200&view=scatterplot&corpus=1d58c9ad21987f6fbb38a73090d4017c'></iframe> | **Pre-Sherlock Holmes Books:** The word cloud of pre-Sherlock Holmes literature highlights a focus on human interactions, emotions, and social hierarchy. Frequent words like “man,” “said,” “cried,” “father,” and “lord” suggest a dialogue-driven narrative with formal address. Bodily descriptors such as “hand,” “face,” and “eyes” emphasize emotional expression, while words like “house” and “room” point to domestic and social settings. This indicates that Doyle’s early works centered on personal struggles and relationships rather than intellectual problem-solving. |
| <iframe style='width: 1112px; height: 673px;' src='https://voyant-tools.org/tool/Cirrus/?visible=200&docId=2749a81ed25292d87f0d823a8029fb76&view=scatterplot&corpus=1d58c9ad21987f6fbb38a73090d4017c'></iframe> | **Sherlock Holmes Books:**The word cloud of Sherlock Holmes literature reflects a focus on investigation, deduction, and dialogue. Frequent words like “Holmes,” “said,” “man,” “case,” and “know” emphasize the central role of the detective and his reasoning process. Terms like “time,” “hand,” and “eyes” suggest attention to observation and detail, essential for solving mysteries. Compared to pre-Holmes works, the setting appears more dynamic, shifting from domestic spaces to crime scenes and moments of action. |
| <iframe style='width: 1112px; height: 673px;' src='https://voyant-tools.org/tool/Cirrus/?visible=200&docId=5ebae079c45f874a11df3273e9852b7a&view=scatterplot&corpus=1d58c9ad21987f6fbb38a73090d4017c'></iframe> | **Post-Sherlock Holmes Books:** The word cloud of post-Sherlock Holmes literature suggests a shift away from detective fiction, returning to themes of human relationships and broader storytelling. Words like “man,” “said,” and “eyes” remain prominent, indicating continued focus on dialogue and character interactions. However, the reduced emphasis on investigative terms suggests a departure from Sherlock Holmes’ analytical style. While some elements of detail and observation persist, the language aligns more with Doyle’s pre-Holmes storytelling approach.|

Before Sherlock Holmes, literature focused on human relationships, emotions, and social hierarchies. Frequent words like "man," "father," "sir," "lord," and "cried" suggest an emphasis on personal interactions and class distinctions, while terms like "hand," "face," and "eyes" highlight bodily gestures and emotional expressions. Settings were grounded in domestic and social spaces, as indicated by words like "house" and "room," reinforcing a narrative style centered on drama and relationships rather than logical reasoning.
With Sherlock Holmes, the focus shifted toward logic and investigation. While dialogue remained prominent ("said"), words like "Holmes," "know," "think," and "asked" suggest a stronger emphasis on intellectual discourse. Observation-based descriptors ("eyes," "face") persisted but served investigative purposes rather than emotional expression. This shift indicates that detective fiction introduced a more analytical, problem-solving approach, transforming narrative style and prioritizing reasoning over sentiment.

### Word Theme Analysis

#### Detective-Related Terms
image

The Sherlock Holmes books (SHB) show a significantly higher use of detective-related terms compared to pre-SH books, with words like case, crime, mystery, investigation, clue, and solution appearing more frequently. This indicates that Doyle refined and popularized the detective genre by making investigative elements central to the narrative. In contrast, post-SH books show a noticeable decline in these terms, suggesting a shift away from detective fiction. While some investigative language remains, it is less frequent and more dispersed, indicating that Doyle moved toward broader storytelling approaches rather than continuing the detective-driven style of Sherlock Holmes.

#### Action and Suspense-Related Terms
image

Action and suspense-related terms were rare in pre-Sherlock Holmes books, moderately present in the Holmes stories, and significantly increased in post-Holmes books. While the Sherlock Holmes series prioritized deduction over action, the post-Holmes era saw a shift toward adventure-driven storytelling, with more frequent use of words like fight, thrill, and chase. This suggests that Doyle’s later works moved away from pure detective fiction, incorporating more action and tension, aligning with the growing popularity of pulp fiction and early thriller novels.

#### Psychological Theme
image

The Sherlock Holmes books introduced psychological themes such as perception, deception, and manipulation, which became more prominent compared to pre-Holmes works. However, post-Holmes books expanded on these elements even further, showing a greater emphasis on psychological complexity. This suggests that while Sherlock Holmes contributed to the development of psychological themes in detective fiction, later works evolved beyond Holmes, deepening and diversifying the exploration of human psychology rather than simply imitating his approach.

#### Law & Justice Terms
image

The bar graph shows an increasing focus on law and justice-related terms throughout Doyle’s works, with a clear rise during the Sherlock Holmes era and an even stronger emphasis in post-Holmes books. While pre-SH books contained some legal references, Sherlock Holmes stories introduced more terms related to justice, trials, and investigations, reinforcing the detective genre’s legal aspects. In post-SH books, the prominence of words like court and judge suggests a shift from detective-driven crime-solving to broader legal and judicial discussions. This indicates that while Sherlock Holmes influenced Doyle’s engagement with law and justice, his later works expanded beyond detective fiction into more structured legal narratives.

#### Character and Role-related Terms
image

The bar graph shows how character and role-related terms evolved across Doyle’s works. During the Sherlock Holmes era, there is a significant rise in words associated with law enforcement, crime, and investigation, such as "inspector," "detective," and "criminal." Pre-SH books also feature "inspector" and "agent" but with less focus on detectives. In post-Holmes books, these detective-related terms decline, while "officer" becomes more prominent, indicating a shift away from detective-driven narratives toward broader authority figures. This suggests that while Sherlock Holmes reinforced Doyle’s engagement with crime and justice themes, his later works moved beyond detective fiction, focusing more on legal and societal structures rather than individual investigations.

## Discussion/Conclusion
### RStudio Conclusion
Our initial hypothesis is that writing Sherlock Holmes influences the works afterward. We expected that many words that did not appear in the books before Sherlock Holmes would recur. This would be seen in the graph by having words closer to the center line between post-SH and Sherlock Holmes Books.

However, this did not turn out to be the case. Both methods of comparing Sherlock Holmes Books (SHB) with pre-Sherlock (pre-SH) and post-Sherlock (post-SH), against pre-Sherlock with post-Sherlock and Sherlock Holmes Books results in minor differences (refer to the graphs above). Using this tool could not give us a concrete answer to our question: does Sherlock Holmes influence Doyle’s work after?

Unlike close reading which allows us to gain very specific insights, distant reading only allows us to gain insights where close reading would be of value (Drucker 115). But, what we do observe is that the themes regarding ‘adventure’ are relevant in all works. But, we conclude that Sherlock Holmes thickens this theme more, observable by how close the word is in pre-SH to post-SH.

Another discovery we observed is the shift in themes between them. Sherlock Holmes Books share a common theme of human anatomy, medicine, and physician practices, judging by how words like ‘arm’, ‘bosom’, and ‘brain’ are relevant in these stories but not the ones after. We suspect that Doyle used these themes because of his physician background. 

By the end of his career, Doyle shifted the themes of his writing to a more political, historical, and war-focused apparent from the more distinctive use of words such as ‘battle’, ‘sword’, and ‘country’. These words could reflect the unwavering conditions of Europe at that time (given how close it was to WW1 and WW2).

### Voyant Tools Conclusion
The  Voyant Tools analysis shows that while the Sherlock Holmes books (SHB) introduced a fast-paced, concise style focused on detective work, logic, and crime-solving, this influence didn’t carry over into Doyle’s later works. Instead, his post-Holmes books shifted toward historical adventure, war, and political intrigue, as seen in the decline of detective-related terms (case, crime, investigation) and the rise of action-driven vocabulary (battle, sword, kingdom).
Sentence structure changed as well—SHB had the shortest sentences (15.8 words per sentence), which suited the detective genre’s need for clarity and precision. In contrast, post-Holmes books had the longest sentences (19.9 words per sentence), pointing to a more descriptive and complex narrative style. Psychological themes like perception, deception, and manipulation remained but expanded beyond detective fiction into broader storytelling. Law and justice themes were still present, but the focus shifted from detective-driven trials to structured legal and political discussions.
Ultimately, the data suggests that while Sherlock Holmes helped shape the detective genre, it was a distinct phase in Doyle’s career rather than a lasting influence on his later writing. His post-Holmes works leaned more toward the themes of his earlier storytelling—adventure, history, and human psychology—rather than investigative crime fiction.

### Overall Conclusion
Our analysis shows that while Sherlock Holmes was a major phase in Doyle’s career, it didn’t permanently change his writing style. Before Holmes, his works explored crime, morality, and supernatural elements. During the Sherlock Holmes era, his writing became sharper and more structured around investigation and logical reasoning. But after Holmes, Doyle shifted focus, moving away from detective fiction and toward historical adventure, war, and politics.
Using  Voyant Tools, we saw a clear drop in detective-related terms in post-Holmes books, while action and suspense elements increased, suggesting a shift toward more dynamic storytelling. Word clouds and frequency graphs helped reveal how common themes like observation and deduction faded in favor of historical and political topics. Meanwhile, Posit.cloud (RMarkdown)highlighted changes in sentence structure, showing that Holmes-era books had the shortest, most concise sentences to suit detective fiction’s clarity, while post-Holmes books had longer, more complex sentences, indicating a shift toward descriptive storytelling. Distinctive word analysis also confirmed that Doyle’s later works introduced different vocabulary, aligning more with adventure and historical fiction.
In the end, Sherlock Holmes refined the detective genre, but it was a distinct phase rather than a defining influence on Doyle’s later works. His post-Holmes books returned to themes more in line with his early storytelling, focusing on adventure, history, and human psychology rather than investigative crime fiction. The combination of computational analysis and human interpretation made it clear that while Holmes left a mark on the mystery genre, Doyle himself moved on.

## Contribution
This article was created by Lucas Lin & Hafizh Ahmad Dahlan. Hafizh developed the research focus and selected the texts, while Lucas structured and designed the document. We divided the analysis, with Hafizh working in Posit Cloud and Lucas using Voyant Tools. After discussing our findings, we collaborated on the conclusion, which Lucas wrote. For reading connections, Hafizh linked the research to Drucker, while Lucas connected it to  Rockwell and Sinclair’s reading. Hafizh wrote the initial background introduction, and we both proofread each other’s work and refined the text to ensure clarity and coherence.

## Resources
* Drucker, Johanna. 2021. The Digital Humanities Coursebook: An Introduction to Digital Methods for Research and Scholarship. 1st ed. Routledge. https://doi.org/10.4324/9781003106531.
* Rockwell, Geoffrey, and Stéfan Sinclair. 2016. The Measured Words: How Computers Analyze Text. University of Illinois Press. https://ieeexplore.ieee.org/document/7580345.

Not ready for grading