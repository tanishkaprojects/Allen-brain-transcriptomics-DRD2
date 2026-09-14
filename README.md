# DRD2 Gene expression mapping across the human brain 

## Summary
This project analyzed how **Dopamine receptor D2 (*DRD2*)** gene expression is distributed across the brain regions using microarray data from the **Allen Human Brain Atlas**. 
The aim of this project was to test whether DRD2 mRNA expression is higher in motor control regions compared to cortical areas. Since Dopamine is involved in controlling physical movement, the mRNA expression is expected to show regional enrichment in the brain's internal motor hubs (Basal ganglia) such as caudate nucleus and putamen compared to Neocortical control layers (The cerebral cortex). Therefore, I analyzed the raw mRNA expression levels on the atlas.

**Main research Question:**
Does DRD2 show stronger expression in brain regions that control movement?

Yes, DRD2 is highly enriched in the basal ganglia mainly in putamen and caudate nucleus while have minimal expression in cerebral cortex. which signifies that it is present abundantly in the movement control regions of the brain. 

---
## Scientific background and hypothesis

* **Why to choose DRD2:** The dopamine D2 receptor (DRD2) is a inhibitory dopamine receptor encoded on chromosome 11.
*  It is one of the most abundant dopamine receptors in the central nervous system
*  It is most abundant in the basal ganglia, nucleus accumbens and prefrontal cortex.
*  Unlike the D1-like receptors which excite neurons, the D2 receptor is inhibitory in nature therefore, plays a major role in central nervous system for suppressing unwanted motor movements and modulating reward-based learning.

  
  ### **Hypothesis:** 
  
As dopamine signaling through DRD2 regulates the motor control. I hypothize that the expression data will show - 

**High expression** i.e. significant structural enrichment (high positive z-scores) inside the basal ganglia specifically the head and tail of the caudate nucleus along with putamen. 

**low expression:** whereas, expression should be zero or negative (z-scores) in the neocortical regions like the cerebral cortex.
  
---
## Methodology 

### Data source
* **Portal:** [Allen Human Brain Atlas] *(https://atlas.brain-map.org/)* 
* **Target Gene:** *DRD2* (Entrez Gene ID: 1813)
* **Selected probe:** CUST_1494_PI417557136
* **Evaluated Regions:** Striatal Structures (Head and Tail of the Caudate Nucleus, Putamen) and Neocortical Controls (Cerebral Cortex).
* **Data Visualization Method:** Data extraction and visualization were performed using the interactive graphic user interface (GUI) of the Allen Human Brain Atlas Web Interface.
  


**Workflow Analysis** 
1. Access the Allen Human Brain Atlas on web (web- interface)
2. Searched for the DRD2 in the search box and selected the human data along with microarray dataset.
3. Extracted the regional expression values using the built in GUI tools
4. Heatmaps and visualisation directly from the atlas portal.
5. Recorded the z-scores for relative enrichment and log2 values for absolute expression.
6. Analyzed data for each regions recorded. 

---

## Neuro-anatomical Visualizations

### Figure 1: Whole-Brain DRD2 Expression Heatmap

![DRD2 Expression Heatmap](images/drd2_heatmap.png)

**Fig 1: Complete microarray matrix from the Allen Human Brain Atlas interface showing DRD2 expression across sampled brain regions.**

### Figure 2: Anatomical Localization of DRD2 mRNA Transcripts

| Macro View: Whole Brain Slice | Micro View: Caudate Head Detail |
| :---: | :---: | 
| ![Macro Overview](images/drd2_macro_overview.png) | ![Caudate Head Zoom](images/drd2_micro_caudal_head_zoomed.png) |

| *Figure 2A: Whole brain slice showing where the striatum tissue block was sampled.* |     *Figure 2B: Zoomed-in tissue section highlighting the caudate head boundary.* |

--- 

## Key findings

**Putamen shows the strongest selective enrichment (Z-score = +3.55) while  nucleus accumbens has the highest 'Absolute mRNA levels' (log2 = 6.14) compared to the rest of the brain.**


### Expression Data

| Brain Region | Subregion | Heatmap Color | Relative Enrichment (Z-Score) | Raw Expression (Log₂ Intensity) 
| :--- | :--- | :--- | :--- | :--- |
| **Basal Ganglia** | Putamen (Front Area) | Bright Red | **3.55274** |  5.58184 | 
| **Basal Ganglia** | Putamen (Back Area) | Bright Red | **2.84138** | 5.01978 | 
| **Caudate Nucleus** | Caudate Body | Dark Red | **2.84814** |  4.93374 | 
| **Caudate Nucleus** | Caudate Tail | Dark Red | **4.00446** |  5.94424 | 
| **Reward Center** | Nucleus Accumbens | Medium Red | **1.4493** | 6.14142 |
| **Cortex** | Cerebral Cortex | Green / Dark green | **-0.87928** | 1.40777 |



---

**Interpretation**

The data shows : 
* All the straital regions (putamen, caudate) shows strong positive z-scores confirming that DRD2 is selective enriched in motor control centres.
* Data revealed that Putamen shows the highest selective enrichment of (+3.55) while the Nucleus Accumbens shows the highest raw expression levels of (6.14). Basal ganglia enrichment links DRD2 to motor disorders such as Parkinson while Nucleus accumbens expression connects the DRD2 to addiction and side effects like Schizophrenia.
* Neocortical areas shows negative expression (-0.87) which proves that DRD2 is under expressed in these regions relative to average of the all brain areas.

---


## Final Discussion

*DRD2* gene activity is heavily concentrated in the basal ganglia. specifically in the Putamen and Caudate Nucleus regions. It has a primary role in controlling movements. While the Putamen shows the highest selective enrichment across the brain (Z = +3.55), the Nucleus Accumbens has the highest overall physical amount of mRNA (log_2 = 6.14). The outer brain regions like the Prefrontal Cortex shows minimal activity (Z = -0.87), proving that DRD2 receptors are strictly localized to deep subcortical areas. This specific pattern explains why D2 receptors are target for movement disorders like Parkinson's disease and schizophrenia disorder. 

---  

## Project access and Repositories 
* **Data Source:** [Allen Human Brain Atlas Portal](https://human.brain-map.org/)
* **Tabular Data** (*https://github.com/tanishkaprojects/Allen-brain-transcriptomics-DRD2/blob/main/drd2-expression-data*)
  Contains Z-scores and log data of the specific regions.

  * **Images** *https://github.com/tanishkaprojects/Allen-brain-transcriptomics-DRD2/tree/main/images*

