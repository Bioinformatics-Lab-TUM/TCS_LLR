# Efficient Alignment-Free Sequence Classification Using k-mer Profiles

This repository contains the implementation of an efficient, alignment-free method for taxonomic classification using k-mer frequency profiles and a log-likelihood ratio (LLR) model. Traditional alignment-based methods often face challenges with large, diverse datasets, especially when sequences have low identity or are distantly related. Our approach overcomes these challenges by leveraging k-mer frequency profiles for computational efficiency without sacrificing accuracy.

## Key Features:
- **Alignment-Free Method**: Classifies biological sequences without the need for sequence alignment, providing better performance on highly diverse datasets.
- **Log-Likelihood Ratio (LLR) Model**: Calculates the likelihood of sequence classification based on the presence of k-mers in taxonomic nodes.
- **Statistical Validation**: Utilizes binomial distribution to calculate p-values, providing statistical significance for classification results.
- **High Accuracy**: Preliminary results show that the method performs closely to traditional alignment-based approaches.
- **Computational Efficiency**: Offers a scalable solution for large datasets, reducing computational complexity.

## How It Works:
1. **k-mer Frequency Profiles**: The method calculates k-mer profiles for sequences, determining the presence or absence of k-mers in specific taxonomic nodes.
2. **Log-Likelihood Ratio (LLR)**: For each k-mer, the LLR is calculated based on its presence in the taxonomic node versus outside it.
3. **Summation and p-value Calculation**: The total LLR is computed by summing LLR values across all k-mers. The statistical significance of results is determined by calculating p-values using a binomial distribution.

## References:
- Zielezinski, Andrzej, et al. (2017). "Alignment-free sequence comparison: benefits, applications, and tools." *Genome Biology*, 18:186. DOI: [10.1186/s13059-017-1319-7](https://doi.org/10.1186/s13059-017-1319-7)
- Zielezinski, Andrzej, et al. (2019). "Benchmarking of alignment-free sequence comparison methods." *Genome Biology*, 20:144. DOI: [10.1186/s13059-019-1755-7](https://doi.org/10.1186/s13059-019-1755-7)

## Authors:
- **Viorel Munteanu**, **Nicolae Drabcinski**, **Dumitru Ciorbă**  
  Department of Computers, Informatics and Microelectronics, Technical University of Moldova
