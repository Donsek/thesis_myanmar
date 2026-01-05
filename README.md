# Thesis_Myanmar

Data exploration for my Master’s thesis on **“Foreign Policy Strategies of Actors in the Myanmar Conflict.”**

The main analysis code can be found in `main.ipynb`.

---

## Data Sources

The data was collected from Telegram channels of the following actors:

- **State Administration Council** (now *State Security and Peace Commission*) — **SAC** — t.me/nationalnewschannel | t.me/hminewai |  t.me/Hno969888
- **National Unity Government** — **NUG** — t.me/nugmyanmar 
- **United Arakan League** — **UAL** — t.me/aainfodesk
- **Palaung State Liberation Front** — **PSLF** — t.me/taangtv2023
- **Karen National Union** — **KNU** — t.me/Karen_Information_Center
- **Karenni Nationalities Defence Force** — **KNDF** — t.me/KNDF_official
- **Chinland National Front** — **CNF** — t.me/Chinlandinformationcenter

The data was initially collected in **JSON format**, then converted into datasets and cleaned.

---

## External Actors Dataset

After preprocessing, a dataset (`external_mentions.csv`) was created containing posts that **only include mentions of the following external actors**:

- China  
- Russia  
- India  
- Western countries (the US, EU, the UK)  
- Bangladesh  
- Thailand  
- ASEAN  
- The UN  
- A number of humanitarian organizations  

For further analysis, the dataset (`mentions_english.csv`) was translated into English using **Google Translate**.

---

## Methodology

**UMAP** was used to project sentence embeddings into a two-dimensional space in order to preserve local semantic neighborhoods. Actor labels were applied *post hoc*, allowing for an unsupervised assessment of discursive proximity between **SAC**, **NUG**, and **EAO** communications.

---

## Visualization

![UMAP](image.png)
