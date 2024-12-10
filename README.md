# **DH2025 Submission**  

**Tracing Antiquity: References to Greco-Roman Authors in Modern Academic Discourse**  

**Authors:**  
Luisa Ripoll-Alberola<sup>1</sup>, Leonardo D’Addario<sup>2</sup>, Manuel Burghardt<sup>1</sup>, Monica Berti<sup>2,1</sup>, Mark Depauw<sup>3</sup>  

<sup>1</sup> Computational Humanities, Leipzig University  
<sup>2</sup> Ancient History, Leipzig University  
<sup>3</sup> Ancient History, KU Leuven  

The project has received funding from the **Horizon Europe Program for Research and Innovation** under **MSCA Doctoral Networks 2022**, Grant Agreement No. **101120349**.  
For more information, visit the project website: [https://mecano-dn.eu/](https://mecano-dn.eu/).  

---

## **Files Overview**  

### **1. `MECANO_authors.csv`**  
This file contains a curated dictionary of **200 prominent ancient authors**, created through a manual mapping of:  
- **Trismegistos Author Gazetteer** — a collection of over 10,000 ancient authors.  
- **L'Année Philologique (APh)** — a bibliographic database of scholarly works on Ancient Greek and Roman authors, founded in 1924 by Jules Marouzeau.  

This file serves as a reference for the most cited and discussed authors in Classical Studies academic discourse.  

#### **Columns**  
- **ID**: Unique identifier for each author.  
- **Author Name**: Name of the author in latinised Greek.  
- **Author Disambiguation**: Notes on author disambiguation (e.g., distinguishing "Dionysios of Halicarnassus" from other authors named "Dionysios").  
- **Perseus Catalog ID**: Corresponding ID from the Perseus Digital Library Catalog (if available).  
- **Wikipedia Entry**: Link to the author's Wikipedia page (if available).  
- **Trismegistos ID**: Identifier of the author in the Trismegistos Gazetteer.  

---

### **2. `aliases.csv`**  
This file builds upon `MECANO_authors.csv` by using the Wikidata Query Service to include **author aliases and spelling variants**, facilitating the recognition of alternative spellings, name variations, and transliterations across different languages and contexts.  

#### **Columns**  
- **Columns from `MECANO_authors.csv`**: (Author Name, Author Disambiguation, Perseus Catalog ID, Wikipedia Entry, Trismegistos ID)  
- **Wikidata ID**: Unique identifier of the author in **Wikidata** (e.g., Q6691 for Homeros).  
- **Aliases**: A list of known spelling variations, translations, and alternate forms of the author's name (e.g., "Homer" for "Homeros").  

This file enables **keyword searching** in Natural Language Processing (NLP) workflows, helping to identify references to authors across texts where name variation occurs.  

---

### **3. `authors_per_discipline.csv`**  
This file provides insights into the **disciplinary prominence of ancient authors**. It lists the top 10 most-cited authors in specific fields of study, alongside a general ranking of the top 10 authors in the entire corpus. This file illustrates how the reception and influence of certain authors shift across various academic disciplines.  

#### **Structure**  
- **Top 10 by discipline**: Identifies the most prominent authors in specific disciplines.  
- **Total top 10**: A general ranking of the most prominent authors in the overall corpus.  
- **Top 10 L'Année Philologique**: A ranking of authors according to the list in `MECANO_authors.csv`, as it is sorted.  

This file supports the analysis of **canonicity** and **disciplinary reception** of classical authors, showing how certain authors are emphasized more in specific academic fields.  

---

## **Citation**  
If you use these datasets, please cite us:  
> **Ripoll-Alberola, L., D’Addario, L., Burghardt, M., Berti, M., & Depauw, M.**  
> *Tracing Antiquity: References to Greco-Roman Authors in Modern Academic Discourse* (under review).  
> Submission for **DH2025**.  

---

## **Contact**  
For questions, issues, or suggestions, please contact **Luisa Ripoll-Alberola** at [ripoll_alberola@informatik.uni-leipzig.de].  
