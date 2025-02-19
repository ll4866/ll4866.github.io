---
title: "Extra Credit"
categories:
  - Extra
tags:
  - Done
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

Key points discussed during the event:
* **K-Anonymity and Extensions:** The event covered k-anonymity, a method that ensures individuals in a dataset cannot be distinguished from at least k-1 others. Extensions like l-diversity and t-closeness were introduced to strengthen privacy by ensuring diversity in sensitive attributes.

* **Challenges of L-Diversity:** L-diversity requires that within an equivalence class, sensitive attributes must have at least l distinct values. However, enforcing this across multiple variables can reduce data utility and effectiveness.

* **Computational Complexity:** Balancing privacy and data utility is computationally difficult. Finding the optimal anonymization approach is an NP-hard problem, meaning it becomes significantly more complex as dataset size increases.

* **Sampling as a Privacy Tool:** Instead of modifying data, sampling introduces uncertainty about whether a person is included in the dataset at all, reducing reidentification risks.

* **Case Study - Fixing Incomplete Anonymization:** A government agency released a dataset without proper documentation or anonymization, leading to privacy concerns. K-anonymity was applied, but significant modifications were necessary to reach a basic level of protection.

* **Data Linkage and Reidentification Risks:** Attackers can use external data sources, such as public records and location tracking, to reconstruct identities from anonymized datasets.

* **Balancing Privacy and Data Utility:** As datasets include more variables, anonymization becomes harder. Striking the right balance requires careful consideration of security measures and data usefulness.

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

## Visuals: 

**Understanding Anonymization Techniques:** A diagram illustrating different anonymization methods, from basic k-anonymity to more advanced techniques like l-diversity and t-closeness.

![This is a Extra Credit How Data Can Be Reidentified image](/assets/images/extra-credit-howDataCanBeReidentified.png "This is a Extra Credit How Data Can Be Reidentified image.")

**How Data Can Be Reidentified:** A visual representation of how attackers can use public data sources to reidentify individuals in anonymized datasets.

![This is a Extra Credit Understanding Anonymization Techniques image](/assets/images/extra-credit-understandingAnonymizationTechniques.png "This is a Extra Credit Understanding Anonymization Techniques image.")

## Course Connection:

This event ties directly to Intro to DAAH, particularly our discussions on what information should and should not be shared with AI tools like ChatGPT. In class, we explored how data is recorded, processed, and the ethical implications of sharing information online. The event reinforced these ideas by showing how even anonymized data can be cross-referenced with external sources to expose private information.

Additionally, we discussed responsible AI use and the risks of improper data handling. If AI models train on datasets that are not properly anonymized, they can inadvertently expose sensitive details. This underscores the importance of carefully managing structured data before sharing or processing it through AI tools.

## Personal Reflection: 

> This event helped me better understand how anonymization works and the risks associated with data privacy. Moving forward, I plan to apply these insights in several ways:
In Future Classes: I will pay closer attention to how data anonymization impacts research and ensure any datasets I use are properly deidentified.
In Capstone Projects: If I work with survey or demographic data, I will explore sampling techniques and penetration testing to assess privacy risks before publishing findings.
In Professional Work: If my career involves data collection or AI, I will prioritize ethical data management to prevent privacy breaches.
This event highlighted the difficulty of balancing privacy with data usability. As data sharing increases, understanding and applying effective anonymization techniques will be essential for maintaining security in research and professional fields.