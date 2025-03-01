---
title: "Extra Credit"
categories:
  - Extra
tags:
  - Done
toc: true
toc_label: "Digital Litaracy Narrative"
toc_sticky: true
---
![This is a Extra Credit Poster image](/assets/images/extra-credit-event.png "This is a Extra Credit Poster image.")

**Event:** [Reducing Risk: An Introduction to Data Anonymization with Kristi Thompson](https://nyu.libcal.com/event/13661742?f=h).
<br/>
**Date:** Mon Feb 10, 2025 
<br/>
**Time:** 9pm - 10:30pm (GST)
<br/>
**Online:** [Zoom Link](https://nyu.zoom.us/j/92900010001).
{: .notice}

## Summary:

Notice: Some sections of this document were refined using AI to enhance clarity and readability while preserving the original meaning.
{: .notice}

Key points discussed during the event:
* **K-Anonymity and Extensions:** K-anonymity is a privacy-preserving method that ensures each individual in a dataset is indistinguishable from at least k−1 others based on certain attributes. However, it has limitations, particularly when sensitive data is involved. To address these limitations, two extensions have been developed: L-diversity and T-closeness. L-diversity ensures that within a group of similar records, there are at least l different values for any sensitive attribute, preventing attackers from easily inferring private information. T-closeness takes this further by ensuring that the distribution of sensitive values within any group is statistically similar to the overall dataset, making it more difficult to extract sensitive insights.

* **Challenges of L-Diversity:** Despite its advantages, L-diversity presents challenges. Enforcing diverse sensitive values can reduce the utility of the dataset, making it less useful for research and analysis. Additionally, in cases where data is sparse, ensuring diversity may require excessive modifications, distorting the original dataset. This creates a trade-off between privacy protection and maintaining meaningful data.

* **Computational Complexity:** As the dataset grows, finding the optimal way to anonymize data becomes increasingly difficult. This is because balancing privacy and data utility is an NP-hard problem, meaning that the computational complexity rises significantly as more data is added. Ensuring that data meets anonymization criteria, such as k-anonymity, l-diversity, or t-closeness, requires intensive processing, especially when dealing with large and complex datasets. Additionally, maintaining privacy while preserving meaningful data becomes more challenging as more attributes and variables are introduced.

* **Sampling as a Privacy Tool:** An alternative approach to anonymization is sampling, where only a subset of the data is included in a study. This introduces uncertainty, making it harder for attackers to determine whether a specific individual's data is present. However, sampling alone is not a foolproof solution, as small datasets may still allow for reidentification if attackers have access to external sources.

* **Case Study - Fixing Incomplete Anonymization:** A real-world case study illustrated the risks of incomplete anonymization. A government agency released a dataset they believed was anonymized, but due to poor documentation and execution, private details could still be inferred. When they later applied K-anonymity, significant modifications were needed to truly anonymize the data. This highlights the importance of designing anonymization strategies before data is released, rather than treating it as an afterthought.

* **Data Linkage and Reidentification Risks:** Even with proper anonymization techniques, data linkage remains a serious risk. Attackers can combine different datasets, such as social media information or public records, to reidentify individuals. A well-known example is the Netflix Prize dataset, where researchers were able to deanonymize supposedly anonymous movie ratings by cross-referencing them with publicly available IMDb reviews. This demonstrates that anonymization is not always foolproof and that external data sources can compromise privacy.

* **Balancing Privacy and Data Utility:** Ultimately, the challenge lies in balancing privacy and data utility. Over-anonymization can strip datasets of valuable insights, making them less useful for research, while weak anonymization increases the risk of reidentification. Researchers must carefully evaluate these trade-offs to determine the right level of anonymization based on the dataset’s purpose and potential risks.

## Resources: 

* K-Anonymity Explained
* L-Diversity and T-Closeness Overview
* Privacy-Preserving Data Sharing Techniques
* Introduction to Data Sampling Methods

No Links to Tutorials or Open Data were provided during the event. However, important terms and concepts discussed
{: .notice}

## Additional Resources: 

* Beginner’s Guide to Data Privacy
* Open Data and Anonymization Techniques
* Penetration Testing for Data Security

No Links to Learning Resources or Beginner Learn were provided during the event. However, important terms and concepts discussed
{: .notice}

## Visuals: 

**Understanding Anonymization Techniques:** A diagram illustrating different anonymization methods, from basic k-anonymity to more advanced techniques like l-diversity and t-closeness.

![This is a Extra Credit How Data Can Be Reidentified image](/assets/images/extra-credit-howDataCanBeReidentified.png "This is a Extra Credit How Data Can Be Reidentified image.")

**How Data Can Be Reidentified:** A visual representation of how attackers can use public data sources to reidentify individuals in anonymized datasets.

![This is a Extra Credit Understanding Anonymization Techniques image](/assets/images/extra-credit-understandingAnonymizationTechniques.png "This is a Extra Credit Understanding Anonymization Techniques image.")

## Course Connection:

This event directly ties into what we’ve been discussing in **Digital Approaches in the Arts and Humanities (DAAH)**—especially the challenges of working with data ethically and effectively.

1. **Data, AI, and Ethical Considerations**
In class, we’ve explored how data is collected, processed, and shared, as well as the risks of anonymization. This event highlighted how even anonymized data can be vulnerable to reidentification, reinforcing the importance of ethical considerations in data handling.  

2. **Computational Complexity and Digital Humanities**
We read Berry and Fagerjord’s *“On the Way to Computational Thinking,”* which talks about the challenges of working with large datasets. This event built on that idea, showing how balancing privacy and data usefulness is a complex problem—not just in anonymization but in digital humanities research in general.

3. **Text Analysis and Data Privacy**
In Rockwell and Sinclair’s *“The Measured Words,”* we discussed how computational tools analyze large text datasets. But as this event showed, privacy risks don’t disappear just because data is stripped of names—attackers can still use patterns and external sources to reidentify individuals.

4. **AI, Large Language Models, and Privacy Risks**
The discussion on data linkage and reidentification connects to our conversations about LLMs and AI ethics. We’ve talked about how AI models are trained on massive datasets—this event made it clear that anonymized data isn’t always as private as it seems, which is a key consideration when using or contributing to AI-driven projects.

## Personal Reflection: 

> Honestly, I didn’t understand much during the event itself. The concepts were technical and overwhelming, and at times, it felt like I was just trying to keep up. However, after going through the screenshots of the slides I took, I was able to piece together a rough understanding of what was discussed. Seeing the key points visually helped me make connections to what we've covered in class, like data ethics and the difficulties of handling large datasets.
> One thing that really stood out was how anonymized data isn’t necessarily safe. I used to assume that removing names and personal details was enough to protect privacy, but this event highlighted how attackers can still reidentify individuals using external data sources. The case study on incomplete anonymization really drove this home—it was surprising to see how even small bits of data can be linked together to expose someone’s identity.
> Going forward, I want to apply these insights in different ways:

> * **In Future Classes:** I’ll be more skeptical about the datasets we use in research, making sure privacy concerns are actually addressed rather than just assuming anonymization is sufficient.
> * **In Capstone Projects:** If I work with survey or demographic data, I’ll explore different anonymization methods beyond k-anonymity—like sampling or differential privacy—to better evaluate how secure the data really is.
> * **In Professional Work:** If I end up working in data collection, AI, or research, I’ll prioritize ethical data management to avoid potential privacy risks.This event made me realize that data security isn’t just an academic issue—it has real-world consequences.

> Something I’m still thinking about is how to balance privacy with data utility. The event made it clear that stronger anonymization can mean losing important details in a dataset. But if we strip too much away, do we risk making the data useless? And if we keep too much, are we sacrificing privacy? These are questions that seem more and more relevant as data-driven technologies continue to advance.
> Overall, this event reinforced that privacy is an ongoing challenge. As technology evolves, so do the methods for reidentification, meaning that anonymization strategies need to keep up. Understanding and applying better anonymization techniques will be crucial—not just for research, but for maintaining security in a world where data is constantly being collected, shared, and analyzed.