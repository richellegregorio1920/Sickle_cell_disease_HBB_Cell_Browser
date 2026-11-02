# From Genome to Cell: Exploring Disease Gene Using the UCSC Cell Browser
This activity uses the UCSC Cell Browser to study human HBB gene expression in single cells. It focuses on exploring a tissue dataset, viewing cell clusters, mapping where HBB is active, and comparing its expression pattern to standard marker genes.

---
# I. UCSC Cell Browser Activity
**Name:** Richelle O. Gregorio  
**Student Number:** 202400734  
* **Assigned Gene:** *HBB* (Hemoglobin Subunit Beta)  
* **Associated Disease:** Sickle Cell Disease (SCD)

Using the same assigned gene (*HBB*) from our previous lab, this activity uses the UCSC Cell Browser to look at *HBB* expression in individual cells and see which cell types or clusters it shows up in.

---
## II. Organ/Tissue Choice and Dataset Information

- **Dataset Name:** Glioblastoma (Cell Browser Dataset ID: `gbm`)
- **Organ/Tissue:** Brain / Human Brain Tumor Tissue (Organs: brain; Diseases: glioblastoma)
- **Organism:** Human (*Homo sapiens*)
- **Lab / Submission:** Kriegstein Lab, UCSF (Submitted by Aparna Bhaduri, 2019-04-22, Version 1)
- **Citation:** BioRxiv preprint (https://www.biorxiv.org/content/10.1101/377606v1.full) / Speir et al., 2021
- **Dataset URL:** [UCSC Cell Browser - Glioblastoma Dataset](https://cells.ucsc.edu/?ds=gbm&label=CellTypeAssignment)

### Why This Dataset Was Selected

Mature red blood cells lose their nuclei and active mRNA, so they cannot be analyzed directly using standard single-cell RNA sequencing. The Glioblastoma dataset was chosen as a surrogate tissue model because its microvascular network retains intact red blood cell precursors within the tumor microenvironment in which enables the visualization of lineage-restricted *HBB* expression across specific cell clusters on the UMAP plot.

![Dataset](screenshots/01_Dataset.png)
***Figure 1.** Selected UCSC Cell Browser Glioblastoma dataset (`gbm`) metadata and cell type cluster map.*

---
## III. Understand The Cell Map
- **A. Visualization Type:** UMAP (Uniform Manifold Approximation and Projection)
- **B. Representation of a Single Dot:** Each dot represents one single measured cell from the glioblastoma tissue sample.
- **C. Meaning of Clusters:** In this dataset, the clusters represent distinct cell types and functional states within the tumor microenvironment (such as cancer stem cells, neural lineages, and vascular/immune cell populations).
- **D. Visible Cell-Type Labels:** 
  - Red Blood Cells
  - Microglia
  - B Cells

 ---
 ## IV. Assigned Gene Expression
- **Assigned Gene Symbol:** `HBB`
- **Dataset Used:** Glioblastoma (`gbm`)
- **Is expression widespread, restricted, or low/undetected?**: Restricted. Instead of spreading across the entire tumor, expression shows up only in specific cell populations.
- **Which cluster(s) appear to contain cells with stronger expression?**: High expression is concentrated in the Red blood cells cluster, with smaller signals present in surrounding microvascular cell lineages like Endothelial cells.
- **Which cluster(s) appear to contain little or no detectable expression?**: Most tumor and brain cell types—including Neuron, Dividing Neuron, Immature Astrocyte, Protoplasmic Astrocyte/Radial Glia, OPC, Microglia, and Tumor Associated Macrophage show no detectable *HBB* expression.

![Gene Expression](screenshots/02_Assigned_gene_expression.png)
***Figure 2.** Single-cell UMAP plot of the Glioblastoma dataset (`gbm`) recolored by HBB gene expression.*

The UMAP plot shows that *HBB* expression is highly restricted rather than widespread. High expression levels are concentrated specifically in the Red blood cells cluster and vascular components like Endothelial cells. In contrast, neural progenitors, astrocytes, microglia, and primary tumor cell types remain completely uncolored, proving that *HBB* functions strictly as an erythroid/vascular lineage marker within this tissue sample.


 
