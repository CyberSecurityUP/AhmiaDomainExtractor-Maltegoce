## Ahmia Domain Extractor

The **Ahmia Domain Extractor** is a Transform for Maltego, specifically designed to extract domains from search results on the Ahmia website. Ahmia is a search tool that indexes, searches, and presents results from domains on the dark web, making this Transform a valuable tool for security researchers, cybersecurity analysts, and professionals involved in digital investigations who require information about activities on the dark web.

### Features
- **Domain Extraction**: Automates the extraction of domains from Ahmia search results, simplifying the data collection process.
- **Unique Filtering**: Ensures that each extracted domain is unique, avoiding duplicates in the results presented in Maltego.
- **Dynamic Response**: Capable of dynamically responding when no domains are found, informing the user through a specific entity in Maltego.

### How It Works
The Transform conducts a search on Ahmia using a term specified by the user. It then parses the HTML of the results page to identify and extract redirect URLs, from which domains are extracted. Each unique domain found is added to the Maltego graph as a separate entity.

### Use Cases
- **Cybersecurity Investigation**: Identify domains related to malicious activities on the dark web.
- **Academic Research**: Collect data for studies on the nature and extent of content available on the dark web.
- **Security Analysis**: Monitor and track domains associated with data leaks, fraud, and other illegal activities.

### Setup
1. Clone the repository of the Transform.
2. Ensure all necessary dependencies are installed.
3. Configure the Transform in Maltego, specifying the correct path for the script and setting the input type as `Phrase`.
4. Run the Transform from a `Phrase` entity with a search term as input.

### Dependencies
- Python 3.x
- Libraries: `requests`, `beautifulsoup4`, `lxml`

### Author
- [Joas A Santos](https://www.linkedin.com/in/joas-antonio-dos-santos/)

This Transform is part of a series of tools designed to enhance the capacity for data analysis and investigation on the dark web, providing quick and accurate insights directly within the Maltego environment.

---
### Screenshots
![image](https://github.com/CyberSecurityUP/AhmiaDomainExtractor-Maltegoce/assets/34966120/8f508eae-ee33-4f1a-8775-4e1850beb3c0)
- Lockbit Research
---
![image](https://github.com/CyberSecurityUP/AhmiaDomainExtractor-Maltegoce/assets/34966120/7d3cfa8c-2b28-4844-a2f2-a9441388e8c6)
- Lockbit and SS7 Attack Research
