# Cytoskeleton and Cell Morphology 

## Student Information & Dataset Metadata
* **Student Name:** Ray Gee Jurac Lisondra
* **Chosen Phenotype:** Peripheral actin
* **Actin Filename:** 07313-actin.DIB
* **DNA Filename:** 07313-DNA.DIB
* **Image Field ID:** 07313
* **Dataset Download Link:** [Broad Bioimage Benchmark Collection (BBBC018)](https://bbbc.broadinstitute.org/BBBC018)

## Fiji Measurement steps
1. Opened the actin channel image (07313-actin.DIB) in Fiji.
2. Configured measurement parameters via **Analyze > Set Measurements...** (checked Area, Mean gray value, and Shape descriptors).
3. Used the **Freehand Selection** tool to manually trace 5 non-overlapping, well-defined cells.
4. Added each cell to the **ROI Manager**, measured the set, and saved the exported data as data/fiji_results.csv.
5. Generated and saved the final annotated micrograph showing all cell outlines to figures/measured_cells.png.

## Analysis Visualizations & Interpretations

### Micrograph Data
* [View Annotated Micrograph (`figures/measured_cells.png`)](figures/measured_cells.png)
  * **Description:** A fluorescence micrograph displaying five individually traced HT29 cells with peripheral F-actin cortical signals.
  * **Interpretation:** Confirms that all traced regions of interest  correspond to well-defined, isolated cells without overlap, serving as the raw spatial baseline for area and signal quantification.

### Cell Area vs. Circularity Scatter Plot
* [View Cell Area vs. Circularity Plot (`results/area_vs_circularity.png`)](results/area_vs_circularity.png)
  * **Description:** A scatter plot mapping Cell Area on the x-axis against Circularity on the y-axis for individual cells.
  * **Interpretation:** All five measured cells exhibit high circularity scores, confirming a consistently round and symmetrical morphology across varying cell sizes. Smaller cells demonstrate slightly higher circularity, whereas larger, more spread cells  show marginally lower circularity due to increased membrane extension and cortical protrusion.

### Mean Actin Fluorescence Intensity Bar Chart
* [View Actin Signal Bar Chart (`results/actin_intensity.png`)](results/actin_intensity.png)
  * **Description:** A vertical bar chart showing the Mean Actin Fluorescence Intensity across each individual traced cell.
  * **Interpretation:** Shows variable F-actin density across the measured population. Cell 1 and Cell 2 exhibit the highest actin signal intensity, indicating dense cortical actin networks and pronounced stress fibers. In contrast, Cells 3, 4, and 5 display progressively lower signal intensities, reflecting heterogenous cytoskeletal expression or varying focal plane depths.

## Four-Question Analysis

### 1. Which specific phenotype did you choose, and what visible features support that choice?
Well-spread, isolated HT29 cells were selected based on distinct F-actin peripheral rings and corresponding nuclear alignment. These visual features ensured accurate tracing of non-overlapping, structurally intact cell boundaries.

### 2. Were your five cells mostly round or elongated? Refer to your circularity and aspect-ratio results.
The measured cells were predominantly round, as indicated by high circularity values averaging near 0.85 and low aspect ratios close to 1.0. These quantitative metrics reflect a symmetrical, unelongated morphology across the sample.

### 3. What role does actin play in maintaining cell shape and in cell movement (Karp Chapter 9)?
Actin microfilaments form the structural cortical network that mechanically supports plasma membrane architecture and maintains cell shape. During motility, dynamic actin polymerization pushes the leading edge forward while actomyosin contraction drives rear translocation.

### 4. Why can a single fixed fluorescence image NOT show how fast a cell moves?
A single fixed fluorescence image captures only a static spatial snapshot, freezing cellular processes at one instant in time. Because calculating speed requires measuring spatial displacement across a time interval, stationary fixed specimens cannot provide the temporal data needed for velocity.

## Data Credit & License Attribution
> Used image set BBBC018v1 from the Broad Bioimage Benchmark Collection (Ljosa et al., Nature Methods, 2012).” The images are licensed CC BY-NC-SA 3.0; retain attribution when sharing image-derived screenshots.
