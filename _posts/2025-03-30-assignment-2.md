---
title: "Historical Data Extration from the Zanzibar Gazette (1909)"
last_modified_at: 2025-04-15T22:00:00-05:00
categories:
  - Assignments
tags:
  - Done
  - AI tools
  - OCR
  - Historical Data
  - Data Visualization
toc: true
toc_label: "Assignment 2"
toc_sticky: true
---
*Written and researched by Ahmad Hafizh and Lucas Lin.*

## Background
### Source Material
For this assignment, we analyzed the Zanzibar Gazette Year 1909. This specific year was chosen due to its high-quality metadata (text-searchable content), visual clarity, and the overall tidiness of its layout compared to earlier issues. We deliberately avoided the years 1914–1918 due to expected publication gaps or inconsistencies caused by World War I.

Within this collection, we explored several tables, including mail schedules, meteorological data, customs reports, principal item exports, and ship sailings. Among these, the **Shipping Reports** caught our attention for two main reasons:
1. They featured a relatively consistent layout and clear quality, making them easier for us—and presumably for machines—to process.
2. Their ease of transcription allowed us to focus on automating the data extraction process and to invest more time in in-depth analysis and visualization.

### Competition Between Machines
One cornerstone that Klein emphasizes is the idea that ‘*the bigger AI model does not mean it is better.*' heir research suggests that simply increasing the volume of data, model complexity, or computational power does not always lead to more accurate AI outputs. For humanities researchers, this insight highlights the limitations of pursuing a single, all-encompassing form of artificial intelligence—revealing the complexity and potential shortcomings of such an approach.

Initially, we used the free version of **ChatGPT-4**  as our primary tool for text recognition. However, we quickly encountered limitations in processing capacity, managing only around five prompts and twenty rows of data. To address this, we shifted to using Google’s <span style="color:blue">`[Gemini](https://gemini.google.com/app)`</span> and <span style="color:blue">`[DeepSeek](https://www.deepseek.com/)`</span>, which provided broader capabilities for our needs.

We began by using the following prompt for Google Gemini:
> **“*Please generate me a table and .csv file for the image shown here.*”**

This prompt allows us to gain two things from the generated outcome. First, by displaying the `.csv` in a table, we can immediately see the result that the AI has generated. This display is important as it will provide us with a quick spot if the AI missed or falsely recognized the text. Second, the .csv file helps us import the data into <span style="color:blue">`[Google Sheets](https://sheets.google.com/)`</span>. We also compared both DeepSeek and Gemini results to see whether they would generate different results. In later parts of our article, we will discuss the pros and cons of both tools.

#### Observations:
After working on our assignment using both Google’s Gemini and DeepSeek, we noted the following:
1. <span style="color:blue">`[Gemini](https://gemini.google.com/app)`</span> 
- The tool lacks support for reading `.csv` files. Since our project heavily relied on this format, this limitation significantly impacted our workflow.
- When performing OCR, Gemini does not apply self-correction. It returns exactly what it reads—even when the output contains errors. As a result, inaccuracies are likely to persist unless manually fixed.
2. <span style="color:blue">`[DeepSeek](https://www.deepseek.com/)`</span>
- In contrast, DeepSeek performs data cleanup. For example, it intelligently interprets ditto marks in tables and fills in repeated values based on preceding rows. We'll showcase several examples of this cleanup later.
- Additionally, DeepSeek can read `.csv` files, which allowed it to reference our existing data structure. This feature proved especially useful, as new OCR outputs could be seamlessly merged with our dataset.

> **🏆 Winner: DeepSeek** takes the crown, as it was able to perform key tasks and deliver results that directly supported our research. It may have been trained on similar datasets, enabling it to recognize and interpret our content more accurately than Gemini. Furthermore, DeepSeek provided unique insights based on our tables—something that would have required significant time and manual effort had we done it row by row.

## Modeling
### Processing the Report
The following is a detailed explanation of our processes. We extracted shipping information from the Zanzibar Gazette 1909 by first screenshotting each page. Then, we fed this image to Google Gemini. Next are the prompts (bold texts) with their respective results that Gemini gave us. Then, we exported this `.csv` data into Google Sheets and created a table by splitting columns. From there, we decided to alter some of the header and data that we deem important to ‘clean’ further manually. 

> **Hello! Can you please generate me a table and .csv based on the image shown?**
Absolutely! Let's break down the information in the image and create a table and a CSV representation.

| ![This is Prompt 1: Table Response.png image](/assets/images/assignment-2/TableResponse.png)  |
|---|
| ![This is Prompt 1: Prompt 1: CSV Response.png image](/assets/images/assignment-2/CSVResponse.png)  |

#### Key Adjustments:
There are several changes that we made before visualizing our data:

1.  **Changing cargo type into ship type**
- We examined that based on the two tables, we can classify the ships into two categories: a cargo ship and a warship (Man-O’-War). Cargo Type, we deem, is unnecessary for our research and would not provide beneficial information. Instead, knowing what type came during a specific week of the month (that is, cargo ships or warships) makes our data much more interesting.
2. **Still in Harbour**
- During our examination, we encountered the phrase *Still in harbour* several times. It usually appears in a ship’s *Bound To* column. We assume that this phrase signifies that the ship has yet to depart from its original harbor. We decided that instead of inputting Still in Harbour, having the original harbor’s name would be better as later on, in our visualization map, no lines are formed since the ship’s location did not change.
3.  **Geographic Data Verification Process**
 - The geocoding phase revealed several categories of location-related challenges that demanded tailored solutions. For completely unrecognizable place names like "German Coast," we conducted archival research to determine appropriate modern equivalents (in this case, "Germany"). Vague directional terms such as "South" were interpreted through careful analysis of shipping routes and contextual clues, typically defaulting to "South Africa" when no clearer alternative emerged. We addressed variable spellings (e.g., "Daressalaam"/"Dar es Salaam") by creating and applying a standardized names reference list. Particularly challenging were obsolete terms like "Tania" and "Gaulle ato Dobouti," which required consultation of historical shipping records and colonial-era documents before we could confidently map them to contemporary equivalents.
4.  **Text Recognition and Formatting Corrections**
- The suboptimal quality of source images necessitated an extensive manual review process for the OCR-generated data. Our team performed side-by-side comparisons of extracted data with original newspaper scans, developing a comprehensive list of common error patterns (e.g., "1900" vs "1909", "Wami" vs "Wani") to guide systematic corrections. We established rigorous formatting standards for ship prefixes (S.S., C.S.), ensuring consistent spacing, punctuation, and proper column assignment through verification against known shipping registries. Company naming conventions were normalized through the implementation of strict formatting rules governing initial spacing (D.O.A.L. vs D. O. A. L.), capitalization standards (Co. vs co.), and punctuation guidelines for ampersands and abbreviations. Every data point underwent double verification to ensure accuracy, particularly for numerical values where OCR frequently misidentified similar-looking digits in low-quality scans.
5.  **Temporal Data Preparation**
- Preparing the date data for Kepler visualization demanded careful precision. We developed a strict standardization process that first reconstructed incomplete dates by analyzing contextual clues from adjacent entries and the newspaper's publication rhythm. Each timestamp was then reformatted to include both date and time components, with empty time values automatically set to 00:00:00. This involved manually processing the entire date column to enforce uniform formatting - every entry was verified to follow the exact "1909-MM-DD 00:00:00" structure, ensuring compatibility with Kepler's visualization requirements. Special attention was given to correcting OCR errors in dates while maintaining historical accuracy throughout the dataset.
6.  **Ship Prefix Standardization Process**
- The inconsistent formatting of ship prefixes (S.S. for steamship, C.S. for cable ship) required extensive manual correction, as they frequently appeared in wrong columns, were omitted entirely, or contained irregular spacing/punctuation (e.g., "S .S.", "S.S ."). We systematically audited each entry, cross-referenced historical registers to verify proper prefixes, and standardized all variations to "S.S." or "C.S." format.

## Data Correction
### A Major Overlook
During three-quarters of the process, we noticed a major oversight from our side when we tried to visualize our data. We took ‘snippets’ of the shipping report by cutting half of the page. However, upon closer inspection, juxtaposing the reports of 16th March 1909 with others, we noticed that all shipping reports of Zanzibar Gazette 1909 occupy full pages.  
>This means that the actual report is not only limited to the cargo ships but also includes warships (categorized as Man-O-War) and smaller traditional vessels (classified as Dhows). In exchange, our data visualization, which was previously limited to cargo ships, was now expanded to include other types of ships.

With this new information in mind, we have decided to include warships in our shipping report table. However, because ‘*Dhows Arrived*’ and ‘*Dhows Departed*’ data were different, we decided not to include them in the table and instead opted to create a separate table and represent it using bar graphs. 

### Nudging the Tool
After having worked on over a hundred rows, fatigue started to envelop our team. We realized that manually editing the rows and columns was not a viable solution. Instead, since we already curated these rows, we thought of something:

>***“What if we feed the machine our edited tabular data and ask them to do OCR and generate the output based on our table structure?”***

At this point, we learned that Gemini did not support .csv files. Luckily, DeepSeek does. The following conversation is the prompts that we use to generate over 100 rows for our table by using DeepSeek.

| Prompt          | Output                                                           |
|-----------------|------------------------------------------------------------------|
| Uploaded 1909_ShippingReport.csv (our base file) Okay. I have attached a file here. Please examine the file and take note of the headers and the contents stored within.           | DeepSeek examines the file.  Let me know if you’d like to explore specific aspects (e.g., filtering by nationality, time ranges, or missing data)! |
| Uploaded a screenshot of the Zanzibar Gazette Shipping Reports 1 June 1909 Now, examine the 1909_ShippingReport.csv file I have provided. If you still remember and examined correctly, you should notice that the tabular data image I have provided you contains data structured similarly to the .csv file I provided. Can you merge the .csv file I just provided with the ones you created? Ignore the longitude (from), latitude (from), longitude (destination), and latitude (destination) columns and leave them empty. | ![Prompt 2.png](/assets/images/assignment-2/Prompt2.png)|
| Remember the steps that you have done previously. Here is a new image similar to the ones I gave before. Extract the textual information and adjust the data so that it fits the 1909_ShippingReport.csv structure while ignoring longitude (from), latitude (from), longitude (destination), and latitude (destination) columns and leave them empty. | ![Prompt 3.png](/assets/images/assignment-2/Prompt3.png)|


### Fantastic Dhows and Where to Find Them
Initially, we tried using Google Sheets to represent our analysis on Dhows. However, we encountered numerous problems regarding Timeline Graphs, and the outcome did not display the data like we expected. Instead, we used an online tool called [CSV Plots](https://www.csvplot.com/) to map our data in a line graph. 

| Dhows Sailed  |
|---------------|
| ![Dhows Sailed](/assets/images/assignment-2/DhowsSailed.png) |

| Dhows Arrived |
|---------------|
| ![Dhows Arrived](/assets/images/assignment-2/DhowsArrive.png) |


## Conclusion
This assignment has allowed us to learn more about AI, specifically its capabilities of doing humanities tasks. On first glance, we did not identify any major conclusions from our data. Rather than not having enough information, it lies at the point that nothing ‘interesting’ comes out of the water. Upon closer inspection, we were able to extract some information, albeit their truth has to be researched further beyond our data. 
Zanzibar was a major maritime trade hub in East Africa. In 1909, it was under British colonial rule but had strong connections to Arabian traders, particularly from Oman. The high number of Zanzibar/British dhows indicates local dominance in maritime activity. We also took into account external influences that might affect the data, such as:
- Seasonal trade routes depended heavily on monsoon patterns from March - May. Dhows from Arabia and India likely followed these seasonal winds. Notable by the drop in dhows arriving.
- The dominance of British/Zanzibari dhows could reflect policies favoring local traders.
- The presence of German dhows could be linked to German East Africa, now countries Rwanda and Burundi, the continental portion of Tanzania, and a small section of Mozambique.
- Arabian and German traders had moderate involvement, while French traders played a minor role.

## Contributions
*On this assignment, Ahmad prompted the AI chatbots, created the .csv file in Google Sheets, made the Dhows graph, and wrote the initial documentation. We both refined the Shipping Report table and collaboratively wrote the markdown post. Lucas focused on the technical aspects, including double-checking the main table, visualizing the data in Kepler, creating a GIF, and proofreading.*

## Resources
Klein, Lauren, et al. "Provocations from the humanities for generative ai research." arXiv preprint arXiv:2502.19190 (2025).
The Editors of Encyclopaedia Britannica. "German East Africa". Encyclopedia Britannica, 15 Oct. 2024, https://www.britannica.com/place/German-East-Africa. 

**✅ Working,,,**
{: .notice}