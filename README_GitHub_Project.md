# Sequence Characteristics of Human TP53 and Gene-Expression Analysis in Breast Cancer (GSE42568)

## Project overview
This one-week bioinformatics mini-project examines (1) nucleotide composition of the human TP53 sequence and (2) exploratory gene-expression differences between breast tumour and normal breast tissue samples in GEO dataset GSE42568.

## Data and tools
- TP53: NCBI Gene, Gene ID 7157, FASTA format
- Breast cancer expression data: NCBI GEO accession GSE42568
- Environment: Google Colab, Python 3
- Tools: Linux utilities (`wget`, `gunzip`, `head`), pandas and matplotlib

## Methods
- Read and validate the TP53 FASTA sequence.
- Count A, T, G and C and calculate GC% and AT%.
- Load the GSE42568 series matrix into pandas.
- Group samples into normal tissue (n=17) and tumour (n=104).
- Calculate group means and tumour-minus-normal differences.
- Visualise the reported top five probe sets.

## Reported TP53 results
- Length: 38,121 bp
- A: 9,925; T: 9,374; G: 9,550; C: 9,272
- GC: 49.37%; AT: 50.63%

## Top five probe sets reported
| Probe ID | Normal mean | Tumour mean | Difference |
|---|---:|---:|---:|
| 201650_at | 6.29 | 11.74 | +5.45 |
| 37892_at | 3.60 | 8.98 | +5.38 |
| 232165_at | 3.84 | 9.12 | +5.28 |
| 201839_s_at | 6.77 | 11.92 | +5.16 |
| 232164_s_at | 4.18 | 9.21 | +5.04 |

## Google Colab notebook
[Open the executable notebook](https://colab.research.google.com/drive/1_JlY3qKyXV1BlOLcYSuGyJPsPOqeJslq?usp=sharing)

## Interpretation
These are exploratory group comparisons. They do not establish causation or confirm gene identity from probe IDs alone. Further annotation and laboratory validation are required.

## Author
Alisha Pandey
