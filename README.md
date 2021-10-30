## Genome Assembly Quality Metrics Tool (GemQT)

GEMQT stands for Genome assEMbly Quality metrics Tool. The corresponding python script evaluates genome/draft assemblies by computing basic metrics. The current tool includes additional metrics alongside to common N50, total assembly size, fragments numbetr etc. The results are saved in a CSV file.


### Arguments

| Argument | Description |
| --- | --- |
| -i, --input | full path to file, in FASTA format (.fasta) containing contigs or scaffolds. |
| -n | values for additional statistics you want to calculate, e.g. 90 for calculation of N90 and L90. |
| -p | optional argument for calculating the percentage of each base. yes/no (default) |
| -o, --output | output's filename that contains the results, without the CSV extension (.csv). |


### Usage

GemQT.py [-h] -i path [-n int [int ...]] [-p yes OR no] -o output_filename

```bash
python GemQT.py -i /users/ckitsoulis/draft_assemblies/genome_assembly.fasta -n 85 90 95 -p yes -o results
```

### Dependencies 

1. [Numpy](https://numpy.org)

2. [Pandas](https://pandas.pydata.org/)

3. [Biopython](https://biopython.org/)

### Notes

The `requirements.txt` file lists all Python libraries that the tool depends on and they will be installed in the environment using the following command:

```bash
pip install -r requirements.txt
```

&nbsp;

&nbsp;


Who:

*[Christos Kitsoulis](https://github.com/ckitsoulis)*

Where:

*Genomics & Bioinformatics group (Genome Nerds) at IMBBC, HCMR*

When:

*During master thesis, October 2021*
