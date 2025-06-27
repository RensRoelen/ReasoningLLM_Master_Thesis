# Beyond Pattern Matching
## A Weighted Entropy Analysis of Functional Specialization in the Llama-2 Architecture

This repository contains the complete experimental framework and results for a Master's thesis investigating functional specialization in Large Language Models. The central finding, that LLMs develop distinct processing pathways for different cognitive tasks, is revealed using a novel weighted entropy methodology designed to accurately measure attention patterns by accounting for attention sink phenomena.

## Research Overview

This study investigates how LLMs adapt their internal processing strategies when faced with different cognitive demands. Using a custom-built weighted entropy metric to correct for attention sinks, the thesis analyzes four 70-billion-parameter Llama-2 variants on two distinct tasks: formal reasoning (mathematics) and functional competence (linguistics). The core finding is that models do not use a single, general-purpose system for problem-solving. Instead, they exhibit a clear "division of labor," developing highly specialized processing pathways for each cognitive domain.

## Key Contributions
This thesis makes two primary contributions: one methodological and one scientific.
- Methodological: Introduces a novel weighted entropy approach that provides a more accurate analysis of attention patterns by accounting for the confounding effects of attention sinks.
- Scientific: Provides strong quantitative evidence for functional specialization in LLMs, showing that models recruit distinct, non-overlapping mechanisms for linguistic vs. mathematical reasoning.
- Theoretical: Challenges a simplistic view of LLMs as monolithic systems, supporting a more nuanced model of emergent modularity where specialized processing patterns develop for different tasks.
- Practical: Offers a complete and reproducible experimental pipeline for analyzing attention entropy in transformer models, from data generation to final analysis.

## Repository Structure

- `datasets/`: Contains the linguistic (sensible/nonsensical) and mathematical (easy/hard) reasoning task datasets used in the study.
- `entropy_llama_snellius.ipynb`: The Jupyter Notebook pipeline for model initialization, data generation, and metric calculation on an HPC service.
- `entropy_llama_truncated.ipynb`: The Jupyter Notebook used for the final statistical analysis, data visualization, and generation of all figures and tables in the thesis.
- `entropy_results_*/`: A directory containing the computed NumPy arrays for weighted entropy, standard entropy, and sink strengths for each model-task combination.


**Author**: Rens Roelen  
**Institution**: University of Amsterdam, MSc Data Science  
**Student Number**: 13210882
