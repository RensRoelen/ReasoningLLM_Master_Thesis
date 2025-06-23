# Beyond Pattern Matching
## A Weighted Entropy Analysis of Functional Specialization in the Llama-2 Architecture

**Attention Entropy Analysis in Llama-2 variants**

This repository contains the experimental framework and results for a Master's thesis investigating attention entropy patterns in large language models, with focus on developing a novel methodology to analyze attention sink phenomena and its impact on reasoning capabilities.

## Research Overview

The study develops a weighted entropy methodology to address attention sink phenomena in transformer models, providing more accurate measurements of attention distribution patterns compared to standard entropy analysis. The research systematically evaluates four major LLM architectures (Llama-2 70B Base/Chat, CodeLlama 70B Base/Instruct) across two reasoning domains: linguistic tasks (sensible vs. nonsensical sentences) and mathematical tasks (easy vs. hard arithmetic problems).

## Key Contributions

- Novel weighted entropy approach that accounts for attention sinks in transformer attention analysis
- Comprehensive evaluation across multiple model architectures and reasoning domains
- Statistical analysis demonstrating systematic differences in attention patterns between reasoning tasks
- Complete experimental pipeline with reproducible methodology for attention entropy analysis

## Repository Structure

- `datasets/`: Linguistic and mathematical reasoning task datasets
- `entropy_llama_snellius.ipynb`: Pipeline for model initialization on HPC service
- `entropy_llama_truncated.ipynb`: Results analysis and visualization
- `entropy_results_*/`: Computed attention metrics for each model-task combination


**Author**: Rens Roelen  
**Institution**: University of Amsterdam, MSc Data Science  
**Student Number**: 13210882
