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
In class, we’ve explored how data is collected, processed, and shared, particularly with AI tools like ChatGPT. This event showed how even when data is anonymized, there’s still a risk of reidentification. This reinforces the importance of data ethics and the need to be mindful of how information is handled.

2. **Computational Complexity and Digital Humanities**
We read Berry and Fagerjord’s *“On the Way to Computational Thinking,”* which talks about the challenges of working with large datasets. This event built on that idea, showing how balancing privacy and data usefulness is a complex problem—not just in anonymization but in digital humanities research in general.

3. **Text Analysis and Data Privacy**
In Rockwell and Sinclair’s *“The Measured Words,”* we discussed how computational tools analyze large text datasets. But as this event showed, privacy risks don’t disappear just because data is stripped of names—attackers can still use patterns and external sources to reidentify individuals.

4. **AI, Large Language Models, and Privacy Risks**
The discussion on data linkage and reidentification connects to our conversations about LLMs and AI ethics. We’ve talked about how AI models are trained on massive datasets—this event made it clear that anonymized data isn’t always as private as it seems, which is a key consideration when using or contributing to AI-driven projects.

## Personal Reflection: 

> Honestly, I didn’t understand much during the event itself. The concepts were technical and overwhelming, and at times, it felt like I was just trying to keep up. However, after going through the screenshots of the slides I took, I was able to piece together a rough understanding of what was discussed. Seeing the key points visually helped me make connections to what we've covered in class, like data ethics and the difficulties of handling large datasets.

One thing that really stood out was how anonymized data isn’t necessarily safe. I used to assume that removing names and personal details was enough to protect privacy, but this event highlighted how attackers can still reidentify individuals using external data sources. The case study on incomplete anonymization really drove this home—it was surprising to see how even small bits of data can be linked together to expose someone’s identity.

Going forward, I want to apply these insights in different ways:

* **In Future Classes:**I’ll be more skeptical about the datasets we use in research, making sure privacy concerns are actually addressed rather than just assuming anonymization is sufficient.
* **In Capstone Projects:** If I work with survey or demographic data, I’ll explore different anonymization methods beyond k-anonymity—like sampling or differential privacy—to better evaluate how secure the data really is.
* **In Professional Work:** If I end up working in data collection, AI, or research, I’ll prioritize ethical data management to avoid potential privacy risks.This event made me realize that data security isn’t just an academic issue—it has real-world consequences.

Something I’m still thinking about is how to balance privacy with data utility. The event made it clear that stronger anonymization can mean losing important details in a dataset. But if we strip too much away, do we risk making the data useless? And if we keep too much, are we sacrificing privacy? These are questions that seem more and more relevant as data-driven technologies continue to advance.

Overall, this event reinforced that privacy is an ongoing challenge. As technology evolves, so do the methods for reidentification, meaning that anonymization strategies need to keep up. Understanding and applying better anonymization techniques will be crucial—not just for research, but for maintaining security in a world where data is constantly being collected, shared, and analyzed.