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
We conducted a distant reading of Sir Arthur Conan Doyle’s works to examine whether the Sherlock Holmes series influenced his later books. Doyle, best known for creating the legendary detective, was a 19th-century British writer whose background in medicine shaped his storytelling, particularly in forensic detail and logical reasoning.
This study investigates whether the themes, vocabulary, and stylistic choices of Sherlock Holmes carried over into Doyle’s later works. Using distant reading techniques, we analyzed a selection of Doyle’s books across three distinct periods—before, during, and after Sherlock Holmes. We employed `Voyant Tools` and `Posit.cloud (RMarkdown)` to track linguistic and thematic shifts across these periods.

## Hypothesis: The Sherlock Holmes Influence  
WWe hypothesize that writing the Sherlock Holmes series influenced Doyle’s later works. If so, his post-Holmes books should share notable similarities with the Holmes stories in vocabulary, themes, or narrative style. Given Holmes' popularity, we expected to see detective fiction elements carried over into Doyle's later works.

## Material Selection & Corpus  
All selected books were chosen based on their time of publication and genre, with a focus on mystery. While Doyle continued to write mystery and detective fiction beyond the Sherlock Holmes series, we focused on the following works to examine his stylistic and thematic evolution.

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

1. **Voyant Tools:** We compiled all books within the same category into a single text file, creating three full-text documents: one for pre-SH, one for SHB, and one for post-SH. These combined texts were then uploaded into Voyant Tools, where we conducted word cloud analysis, frequency distributions, and general textual analysis to identify recurring terms and themes across different time periods.
2. **Posit.cloud (RStudio, ggplot2):** Used for in-depth statistical analysis, including graphical representations of recurring terms. Key analyses included:
  * `Identifying the Most Distinctive Words in Three (Sets of) Texts Compared` - compared vocabulary differences between pre-SH, SHB, and post-SH books.
  * `Summarizing a text from Project Gutenberg in a word cloud` - Created visual representations of each corpus to highlight dominant themes.

This method follows the ideas discussed in Rockwell and Sinclair’s "The Measured Words: How Computers Analyze Text", which explains how computational tools recognize patterns rather than interpret meaning. While these tools helped us detect trends in Doyle’s writing, we applied human interpretation to refine our conclusions and gain a more nuanced understanding of the data.

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

The data reveals that Doyle’s writing evolved after Sherlock Holmes, with post-Holmes works having the highest word count and longer sentences, indicating a shift toward more descriptive storytelling. Sherlock Holmes books feature shorter sentences, reinforcing their fast-paced detective style. Despite these differences, Doyle’s vocabulary range remained stable, as seen in the consistent 6% type-to-word ratio. However, the data does not strongly suggest that post-Holmes works retained the stylistic influence of Sherlock Holmes, implying a deliberate narrative shift in Doyle’s later writing.

<iframe style='width: 1112px; height: 673px;' src='https://voyant-tools.org/tool/ScatterPlot/?docId=81a2da64a1c005e22b2471173ef02741&docId=2749a81ed25292d87f0d823a8029fb76&docId=5ebae079c45f874a11df3273e9852b7a&limit=206&dimensions=2&label=docs&label=summary&view=topics&corpus=1d58c9ad21987f6fbb38a73090d4017c'></iframe>

The scatter plot reveals distinct stylistic shifts in Doyle’s writing across different phases. The clustering of Sherlock Holmes books and Pre-Holmes works suggests that Doyle retained certain stylistic traits despite shifting to detective fiction. However, the Post-Holmes books are positioned farther from the Holmes stories, indicating a notable departure in style and a move toward a different literary direction. Despite this shift, alignment along the Y-axis suggests lingering stylistic influences, such as sentence complexity. This supports the idea that the Sherlock Holmes series was a distinct phase in Doyle’s career rather than a permanent stylistic transformation.

### Word Theme Analysis
#### Detective-Related Terms
image
The Sherlock Holmes books exhibit a significantly higher frequency of detective-related terms—such as case, crime, mystery, and investigation—compared to Doyle’s pre-Holmes works. This suggests that Doyle refined and popularized the detective genre by making investigative elements more central. However, post-Holmes books show a marked decline in these terms, indicating a shift away from detective fiction. While some investigative language persists, its reduced frequency and dispersion imply that Doyle transitioned toward broader storytelling approaches rather than continuing the detective-driven style of Sherlock Holmes.
#### Action and Suspense-Related Terms
image
Action and suspense-related terms were minimal in Doyle’s pre-Holmes works, moderately present in the Sherlock Holmes stories, and significantly increased in post-Holmes books. While Holmes’ narratives emphasized deduction over action, Doyle’s later works leaned toward adventure-driven storytelling, incorporating more frequent mentions of fight, thrill, and chase. This shift suggests a departure from pure detective fiction, aligning with the rise of pulp fiction and early thriller genres.
#### Psychological Theme
image
Sherlock Holmes introduced psychological themes such as perception, deception, and manipulation, making them more prominent than in Doyle’s pre-Holmes works. Post-Holmes books expanded even further on these elements, emphasizing psychological complexity. This suggests that while Holmes played a crucial role in shaping psychological themes in detective fiction, later works evolved beyond imitation, deepening the exploration of human psychology.
#### Character and Role-related Terms
image
The bar graph illustrates the evolution of character and role-related terms in Doyle’s works. During the Sherlock Holmes era, terms like "inspector," "detective," and "criminal" rise significantly, reflecting a strong focus on investigation. Pre-Holmes books feature "inspector" and "agent" but with less emphasis on detectives. Post-Holmes, detective-related terms decline as "officer" becomes more prominent, marking a shift from detective-driven narratives to broader authority figures. This suggests that while Holmes reinforced Doyle’s engagement with crime and justice, his later works shifted toward legal and societal themes over individual investigations.

## Discussion/Conclusion
### RStudio Conclusion
Our initial hypothesis was that writing Sherlock Holmes influenced Doyle’s later works. We expected words that were absent before Sherlock Holmes to recur afterward, appearing closer to the center line between post-Holmes and Sherlock Holmes books in our analysis. However, the data did not support this assumption. Comparing Sherlock Holmes books (SHB) with both pre-Sherlock (pre-SH) and post-Sherlock (post-SH) works showed only minor differences. Thus, this computational approach could not definitively answer whether Sherlock Holmes influenced Doyle’s later writing.
Unlike close reading, which provides specific insights, distant reading offers broader patterns that require further interpretation (Drucker 115). However, our findings reveal that the theme of ‘adventure’ is present in all of Doyle’s works, though Sherlock Holmes deepens this theme, as evidenced by its closer alignment between pre-SH and post-SH texts. Another significant discovery is the thematic shift across different periods. Sherlock Holmes books prominently feature human anatomy, medicine, and physician-related terms—such as ‘arm,’ ‘bosom,’ and ‘brain’—likely influenced by Doyle’s medical background. By the end of his career, Doyle’s works shifted toward political, historical, and war-focused themes, seen in the increasing use of words like ‘battle,’ ‘sword,’ and ‘country.’ This shift may reflect the political climate of Europe, given its proximity to WWI and WWII.
The `Voyant Tools` analysis further illustrates this evolution. While Sherlock Holmes books were concise and fast-paced, centered on detective work, logic, and crime-solving, this influence did not persist in Doyle’s later works. Post-Holmes books instead emphasized historical adventure, war, and political intrigue. Detective-related terms (such as ‘case,’ ‘crime,’ and ‘investigation’) declined, while action-driven vocabulary (‘battle,’ ‘sword,’ ‘kingdom’) rose. Sentence structure also changed—SHB had the shortest sentences (15.8 words per sentence), aligning with detective fiction’s need for clarity, while post-Holmes books had the longest (19.9 words per sentence), indicating a more descriptive, complex narrative style. Psychological themes like perception and deception remained, expanding beyond detective fiction into broader storytelling. While law and justice themes persisted, they transitioned from detective trials to structured legal and political discussions.
Overall, our analysis shows that while Sherlock Holmes was a pivotal phase in Doyle’s career, it did not permanently alter his writing style. Before Holmes, his works explored crime, morality, and the supernatural. During the Holmes era, his writing became sharper and centered on investigation and logical reasoning. However, after Holmes, Doyle moved away from detective fiction, favoring historical adventure, war, and politics.
Using `Voyant Tools`, we observed a decline in detective-related terms post-Holmes, while action and suspense elements increased, indicating a shift toward dynamic storytelling. Word clouds and frequency graphs highlighted how themes of observation and deduction faded in favor of historical and political topics. Meanwhile, `Posit.cloud (RMarkdown)` revealed changes in sentence structure, with Holmes-era books featuring shorter, more concise sentences, while post-Holmes books had longer, more complex structures suited to descriptive storytelling. Distinctive word analysis confirmed Doyle’s later vocabulary aligned more with adventure and historical fiction.
Ultimately, Sherlock Holmes refined the detective genre, but it was a distinct phase rather than a defining influence on Doyle’s later works. His post-Holmes books returned to themes more in line with his early storytelling—adventure, history, and human psychology—rather than investigative crime fiction. Through computational analysis and human interpretation, we conclude that while Holmes left a mark on the mystery genre, Doyle himself moved on.

## Author Contributions
This article was co-authored by Lucas Lin and Hafizh Ahmad Dahlan. Hafizh developed the research focus and selected the texts, while Lucas structured and designed the document. The analysis was divided between them: Hafizh conducted research using Posit Cloud, while Lucas analyzed data with Voyant Tools. After discussing their findings, they collaborated on the conclusion, which Lucas drafted. For theoretical connections, Hafizh linked the research to Drucker, while Lucas referenced Rockwell and Sinclair. Hafizh wrote the initial background introduction, and both authors proofread and refined the text for clarity and coherence.

## Resources
* Drucker, Johanna. 2021. The Digital Humanities Coursebook: An Introduction to Digital Methods for Research and Scholarship. 1st ed. Routledge. https://doi.org/10.4324/9781003106531.
* Rockwell, Geoffrey, and Stéfan Sinclair. 2016. The Measured Words: How Computers Analyze Text. University of Illinois Press. https://ieeexplore.ieee.org/document/7580345.

Not ready for grading