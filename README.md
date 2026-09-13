# Gene expression mapping of Dopamine receptor D2 (DRD2) across the human brain 

## Summary
In this project, I worked on how the brain maps out its genetic blueprints for movement. I observed **Dopamine receptor D2 (*DRD2*)** across the entire human brain using high-resolution molecular data. I took microarray transcriptome dataset from the **Allen Human Brain Atlas**
The aim of this project is to test whether DRD2 gene activity matches the brain's known movement control centers. Since Dopamine is involved in controlling physical movement, the mRNA expression is expected to show regional enrichment in the brain's internal motor hubs (Basal ganglia) such as caudate nucleus and putamen compared to Neocortical control layers (The cerebral cortex). Therefore, I analyzed the raw mRNA expression levels on the atlas.

---
## Scientific background and hypothesis

* **Biological context:** The dopamine D2 receptor (DRD2) is a crucial G protein-coupled receptor encoded by the DRD2 gene on chromosome 11. It is one of the most abundant dopamine receptors in the central nervous system and is particularly concentrated in the basal ganglia, nucleus accumbens, and prefrontal cortex. Unlike D1-like receptors which excite neurons, the D2 receptor is inhibitory. It plays a major role in central nervous system for inhibiting unwanted motor actions and modulating reward-based learning. 
* **Hypothesis:** Because DRD2 is heavily involved in gating the motor signals, I hypothize that the raw expression data will reveal significant structural enrichment (high positive z-scores) inside the basal ganglia specifically the head and tail of he caudate nucleus. whereas, expression should be zero or negative (z-scores) in the neocortical regions like the cerebral cortex.
  
---
## Methodology & Data Sources
* **Data Source:** [Allen Human Brain Atlas] *(https://atlas.brain-map.org/)* (Microarray Transcriptomic Data).
* **Data Visualization Method:** Data extraction and regional visualization were performed using the interactive graphic user interface (GUI) of the Allen Human Brain Atlas Web Interface.
* **Target Gene:** *DRD2* (Entrez Gene ID: 1813)
* **Selected probe:** CUST_1494_PI417557136
* **Evaluated Regions:** Striatal Structures (Head and Tail of the Caudate Nucleus, Putamen) and Neocortical Controls (Cerebral Cortex).
---

## Neuroanatomical Visualizations

### Figure 1: Whole-Brain DRD2 Expression Heatmap

![DRD2 Expression Heatmap](drd2_heatmap.png)

**Fig 1: Complete microarray matrix view from the Allen Human Brain Atlas interface tracking the DRD2 expression profiles across human donor tissue.**

### Figure 2: Anatomical Localization of DRD2 mRNA Transcripts

| Macro View: Whole Brain Slice | Micro View: Caudate Head Detail |
| :---: | :---: | 
| ![Macro Overview](drd2_macro_overview.png) | ![Caudate Head Zoom](drd2_micro_caudal_head_zoomed.png) |

| *Figure 2A: Whole brain slice showing where the striatum tissue block was sampled.* |     *Figure 2B: Zoomed-in tissue section highlighting the caudate head boundary.* |

--- 

## Key findings

### Expression Data

| Brain Region | Subregion | Heatmap Color | Relative Enrichment (Z-Score) | Raw Expression (Log₂ Intensity) 
| :--- | :--- | :--- | :--- | :--- |
| **Basal Ganglia** | Putamen (Front Area) | Bright Red | **3.55274** |  5.58184 | 
| **Basal Ganglia** | Putamen (Back Area) | Bright Red | ** 2.84138** | 5.01978 | 
| **Caudate Nucleus** | Caudate Body | Dark Red | **2.84814** |  4.93374 | 
| **Caudate Nucleus** | Caudate Tail | Dark Red | **4.00446** |  5.94424 | 
| **Reward Center** | Nucleus Accumbens | Medium Red | **1.4493** | 6.14142 |
| **Cortex** | Cerebral Cortex | Green / Dark green | **-0.87928** | 1.40777 |

**Putamen shows the strongest selective enrichment (Z-score = +3.55) compared to the rest of the brain.**

---

**Main takeaways from this project**


* The Putamen shows the highest selective enrichment of (+3.55) while the Nucleus Accumbens shows the highest mRNA levels of (6.14)
* Neocortical areas shows negative expression (-0.87) which proves that they are present mainly in sub-cortical regions.
* The localization of D2 receptors alters the motor/limbic circuits and therefore affecting the body's movement and causes side effects like Parkinson.

---


## Discussion

*DRD2* gene activity is heavily concentrated in the basal ganglia. specifically in the Putamen and Caudate Nucleus regions. It has a primary role in controlling movements. While the Putamen shows the highest selective enrichment across the brain (Z = +3.55), the Nucleus Accumbens has the highest overall physical amount of mRNA (log_2 = 6.14). The outer brain regions like the Prefrontal Cortex shows minimal activity (Z = -0.87), proving that DRD2 receptors are strictly localized to deep subcortical areas. This specific pattern explains why D2 receptors are target for movement disorders like Parkinson's disease and schizophrenia disorder. 

---

## Project access and Repositories 
* **Data Source:** [Allen Human Brain Atlas Portal](https://human.brain-map.org/)
* **Tabular Data** (*https://github.com/tanishkaprojects/Allen-brain-transcriptomics-DRD2/blob/main/drd2-expression-data*)
  Contains Z-scores and log data of the specific regions.

  * **Visual data**

