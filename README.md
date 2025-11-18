# Plastid-5UTRs
Code for manuscript titled:
Deep learning-based investigation of chloroplast translation regulatory sequences
DOI: https://doi.org/

# Overview
We developed and applied an optimized hybrid CNN–LSTM–Attention–Residual deep learning model to classify and analyze 5′ untranslated region (UTR) sequences from plant and algal chloroplasts.

Our model is an improved version of a previous framework developed for the chloroplast genome (Nature Scientific Reports, 2025). It achieved near-perfect prediction accuracy in classifying plant and algal leader sequences, including those with and without Shine–Dalgarno (SD) motifs across both groups.

This approach provides new insights into the architecture of chloroplast translation regulatory elements without relying on prior assumptions about known regulatory regions. By integrating advanced interpretative techniques—such as attention heatmaps, saliency mapping, and perturbation tests—we offer transparent explanations of the model’s decision-making process.

From an applied perspective, the results obtained from this hybrid model suggest practical strategies to improve transgene translation efficiency. These include identifying functional plant-driven heterologous leader sequences (publicly released in this article) and generating hybrid leader sequences that combine plant and algal regions for algal plastomes. Such findings may significantly enhance both fundamental understanding and applied research in chloroplast genetic engineering.

Building on previous work (https://www.nature.com/articles/s41598-025-12796-9), this manuscript reports the first deep learning model focused specifically on plastid translational regulatory sequences.

# Authors
Mohammad Ali Abbasi-Vineh¹*, Pär K. Ingvarsson²*, Naser Farrokhi¹*

¹ Department of Cell & Molecular Biology, Faculty of Life Sciences & Biotechnology, Shahid Beheshti University, Tehran, Iran
² Department of Plant Biology, Swedish University of Agricultural Sciences, Uppsala, Sweden

*Correspondences

# Requirements and Installation
All analyses were conducted using the free version of the Kaggle platform, which provides cloud-based computational resources. Alternatively, the code can be run in Google Colaboratory (Colab) or any offline Python-based environment.

All necessary dependencies and packages are specified within the code and can be installed easily using standard package management tools.

# Availability of the Code
All scripts used in this study are provided in "Main_Scripts_5′_UTR.ipynb".

Key sections of the notebook include annotations such as:

The code to run the CNN-LSTM-Attention-Residual hybrid model

The code to have the Confusion matrix

The code to have the ROC and PR curves

The code to have the analysis of attention heatmaps

The code to have the Perturbation test analysis

The code to have the Group saliency map analysis

These modular and well-commented sections allow users to quickly locate and adapt relevant parts of the code for their own applications.

# Biological Interpretation of CNN–LSTM–Attention–Residual Components
1. Convolutional Neural Networks (CNNs) — Pattern Scanners
CNN layers scan input sequences using small “windows” (kernels) that move along the sequence to detect local patterns such as DNA motifs or conserved nucleotide groups. This is analogous to a biologist scanning a DNA fragment for regulatory signals. For example, a kernel of size 5 examines every 5-nucleotide segment, identifying recurring motifs important for classification.

2. Residual Connections — Memory Shortcuts
Residual connections act as shortcuts that preserve key features from earlier layers, preventing the loss of critical information during multi-layer processing. This resembles a researcher retaining early observations to reference later in an analysis.

3. Long Short-Term Memory (LSTM) Layers — Sequence Memory
LSTM layers maintain information across long distances in sequences, capturing dependencies between distant nucleotides or elements. For instance, they can model how a base at position 10 influences a motif at position 250.

4. Attention Mechanisms — Spotlight on Important Regions
Attention layers assign greater weight to sequence positions that strongly influence classification outcomes. This mechanism mirrors how a biologist focuses on regulatory hotspots during sequence analysis.

5. Fully Connected Layers — Decision Making
The fully connected layers integrate learned features into final predictions, much like a scientist drawing conclusions after examining all evidence.

Summary
This biologically grounded explanation bridges the gap between complex deep learning concepts and biological understanding, making the hybrid model accessible to molecular geneticists and computational biologists alike.

# Model Flexibility
The current hybrid model is highly adaptable. Researchers can modify sequence length, adjust layer depth or unit size, and apply it across varied omics datasets. This flexibility makes it suitable for both exploratory and applied research scenarios.

# Citations
If you use the data augmentation approaches or models presented in this repository, please cite:

Abbasi-Vineh, M.A., Ingvarsson, P.K., Farrokhi, N., et al.
Deep learning-based investigation of chloroplast translation regulatory sequences.
Nature Scientific Reports (2025). DOI: https://doi.org/10.1038/s41598-025-12796-9

Contact
For technical questions or additional details regarding data or analysis, please contact:

Mohammad Ali Abbasi-Vineh*: ali.abbasi@modares.ac.ir; ali.abbasi1568@yahoo.com

Naser Farrokhi*: n_farrokhi@sbu.ac.ir

Pär K. Ingvarsson*: par.ingvarsson@slu.se

*Correspondences

