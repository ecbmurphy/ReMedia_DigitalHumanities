<img src="./Re_Colour.png" alt="ReMedia logo is the letters RE in a green cirlce." width="175">

# ReMedia Infrastructure for Research and Creation - Projects
Features publicly available data, scripts, and documentation for digital humanities research.
---

## 🔗 Links

[See this portfolio in the repository](https://github.com/ecbmurphy/ReMedia_DigitalHumanities/edit/main/README.md)
<br>[ReMedia Website](https://www.https://remediaresearch.ca/)

---

## About ReMedia

In ReMedia we study multimedia cultural memory: what we remember about culture, how we remember it, and how technology and media shape that memory. We take a "problem-centered," case-study approach to research. The projects below contain data, scripts, and documentation from case studies created by research partners and student research assistants. Scroll down for data related to digital humanities pedagogy. 

This portfolio provides descriptions of data building, web scraping, and computational analysis projects in ReMedia and led by the PI, Dr. Emily Christina Murphy. Some projects featured here are in-progress, and others are cleaned, completed, or on-hiaitus. This public-facing repository does not include any sensitive of living subject data. In ReMedia our primary data repository is Microsoft Teams on secure UBCO servers. If you have questions about these projects or curious to see more, please get in touch with the PI at emily.murphy@ubc.ca. 

---

## 🟢 Featured Research Projects

### 1. 🟢 [Modernist Remediations -- Goodreads data for Iconic Biography book](https://github.com/OdessyLiu/Modernist_Remediation_ReMedia/tree/main/Data/Goodreads_Comics_Data)
**Description:** A brief description of the project and what it does. Mention any key technologies or tools you used.

- **Tech Stack:** [Python, .csv, jsLDA, Word2Vec]
- **Features:**
  - Metadata on graphic biographies with unique identifiers, UML
  - Coming soon: scraped data from Goodreads
  - Coming soon: scripts for webscraping and analysis

---

### 2. 🟢 [Modernist Remediations -- Twitter data from collaboration with Science Museum London]()
**Description:** A brief description of the project and its purpose.

- **Tech Stack:** [Python, Flask, PostgreSQL]
- **Features:**
  - Feature 1
  - Feature 2
  - Feature 3

---

### 3. 🟢 [Feminism, Modernism, and Ego-Network](https://github.com/ecbmurphy/FeminismModernismEgoNetwork)
- **Tech Stack:** Neo4j, Gephi

**Description:** 
This project was the topic of a SSHRC postdoctoral fellowship at the University of Victoria with the Linked Modernisms project, a Mellon-funded fellowship at the Harry Ransom Centre at the University of Texas at Austin, and a Hampton New Faculty Grant at the University of British Columbia. “Modernism, Feminism, and the Ego-Network” applies linked open data technologies to the personal, professional, and artistic networks of early-twentieth century women writers and editors. It asks two research questions: (1) How can contemporary technologies and social networks change how we understand the nature of women’s artistic and cultural contributions? (2) How can the study of women’s personal and artistic networks change the way we develop technologies for literary and historical inquiry? 

Linked open data is a metadata standard that may be structured to “[allow] metadata to be connected and enriched…and links made between related resources” (“Europeana Linked Open Data”), and underpins linked resources in the Semantic Web. Most linked data projects construct a whole network and measure the importance of individual notes in a network through measures like degree, closeness & betweenness centrality. In this project my goal was to experiment with modeling "ego-networks," or sets of relationships that are all connected through a single node -- in this case a person, modernist editor, author, activist, socialite, and muse, Nancy Cunard. 

At the Harry Ransom Centre, my archival research focused on the Cunard collection, recording all of the connections represented by her letters. You'll find that data in Letters.csv. Here is a visualization produced in Gephi that includes all of the nodes and edges represented by all letters sent and received. 

- Persons are orange
- Letters are beige
- Poems included in letters are red

<img src="https://github.com/ecbmurphy/FeminismModernismEgoNetwork/blob/master/Nancy1.png" alt="All nodes and edges from letters metadata." width="300">

The nodes in this case are people with whom Cunard exchanged letters. These results simply confirm the premise of the project, which is that Cunard is the central node of her own ego-network, represented by the letters. 

In the next phase of the project, student research assistant Meredith Lister and I translated the tabular format .csv data from the letters into a Neo4j database format. We also expanded the project to consider how the letters related to Cunard's anthology _Poems for France_(1941). Anthology forms offer an interesting case study in the role of editors in literary production, and although most studies of modernist editing focus on figures like T.S. Eliot and Maxwell Perkins, the role of women as the "midwives of modernism" (Benstock) was often effected through editing. Most of Cunard's cultural contributions were anthologies and collections, and her insufficient treatment in in modernist literary studies may result from this very multiplicity. 

In combining Cunard's letters with one of her smaller anthologies, my goal was to find a way of representing literary history focused on a figure that facilitated mediated community connection. I therefore modelled data that recorded anthologized poems, all correspondence related to those poems, and all correspondence related to anthology that did not align with a poem. You can find that dataset in the [0PoemsForFrancePrototype.xslx file](https://github.com/ecbmurphy/FeminismModernismEgoNetwork/blob/master/0PoemsForFrancePrototype.xlsx) in this repository. Our first visualization included all persons, poems, publications, and letters is similar to the letters-only network visualization. 

- Persons are orange
- Poems are red
- Publications are blue
- Letters are beige

<img src="https://github.com/ecbmurphy/FeminismModernismEgoNetwork/blob/master/send%20receive%20letters.png" alt="All nodes and edges from letters metadata." width="300">

We produced of the most interesting visualizations by removing all letters directly received or sent by Cunard. This is the result, in which Cunard is the connected orange person node in the top left. The central blue publication node in the middle surrounded by red poem nodes is the anthology _Poems for France_. 

<img src="https://github.com/ecbmurphy/FeminismModernismEgoNetwork/blob/master/Nancy2.png" alt="Visualization of Cunard anthology without letters directly to or from Cunard" width="300">

The force-directed graph does not have any inherent meaning: the algorithm is simply trying to avoid overlapping edges, and the location of the nodes in space does not indicate any particular relationship among nodes without explicit edges. However, what is most interesting to me is the way that this visualization creates a kind of ego-network around the anthology and that, even though Cunard does not publish in the anthology, she still remains one of the most connected person nodes. The outer ring of unconnected nodes represent poems and persons mentioned in the dataset (in letters, primarily) and collections that the poems also appear in. It suggests to me a kind of ghost network of publications and literary works. 

- **Next steps:**
This project is on hiaitus. Next steps will include expanding the data model from _Poems for France_ to Cunard's larger and more famous anthologies. I am curious to know how far the concept of an ego-network can actually take this work. I anticipate that adding more anthologies and revealing more "ghost networks" might mean that I need to balance ego-network modelling approaches with validated whole-network analysis like centrality and betweenness. 

---

### 4. 🟢 [LinkedModernisms](https://github.com/orgs/LinkedModernismProject/repositories)
**Description:** A summary of what this project is about and any challenges you faced.

- **Tech Stack:** JSON, CSV, Python, Apache Jena, Neo4j, SPARQL, RDFXML
- **Features:**
  - Feature 1
  - Feature 2
  - Feature 3

---

## 🟣 Featured Digital Humanities Pedagogy Projects

### 5. 🟣 [DIHU407: Media and Contemporary Readers](https://github.com/yourusername/project-repo)
**Description:** A summary of what this project is about and any challenges you faced.

- **Tech Stack:** [Angular, Firebase]
- **Features:**
  - Feature 1
  - Feature 2
  - Feature 3

---

### 6. 🟣 [Contract Grading Resources for IJHAC article](https://github.com/yourusername/project-repo)
**Description:** A summary of what this project is about and any challenges you faced.

- **Tech Stack:** [Angular, Firebase]
- **Features:**
  - Feature 1
  - Feature 2
  - Feature 3

---

### 7. 🟣 [Coming Soon: Repository Material for EnTwine edited collection](https://github.com/yourusername/project-repo)
**Description:** A summary of what this project is about and any challenges you faced.

- **Tech Stack:** [Angular, Firebase]
- **Features:**
  - Feature 1
  - Feature 2
  - Feature 3

---

## 📧 Contact

If you'd like to collaborate or discuss my work, feel free to reach out:

- **Email:** [your.email@example.com](mailto:your.email@example.com)
- **GitHub:** [github.com/yourusername](https://github.com/yourusername)
- **Website:** [your-website.com](https://your-website.com)

---

Thank you for visiting my portfolio! Looking forward to connecting and building great things together!
