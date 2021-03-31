# POGENOM #
POGENOM (POpulation GENOmics from Metagenomes) is a computer program that calculates several population genomic parameters for a genome in relation to a set of metagnome samples.

![POGENOM image, courtesy Samuel Salminen](https://github.com/EnvGen/POGENOM/pogenom.jpg)

## Description ##
POGENOM takes as input a file of the variant call format (VCF). This is generated by mapping one or several metagenome samples against a reference genome with a read aligner and calling variants using a variant caller. The Input_POGENOM pipeline can be used to generate the input. POGENOM calculates the nucleotide diversity, 𝜋, within each sample. If multiple samples have been mapped, the fixation index (FST) is calculated for all pairs of samples. If in addition to the VCF file an annotation file of the General Feature Format (GFF) is provided, gene-wise 𝜋 and FST will be calculated. If, further, the genome sequence is provided in the GFF file or in a separate FASTA file, amino acid frequencies will be calculated for each codon position in each gene and sample, and gene-wise 𝜋 and FST will be calculated also at the amino acid level. Now also non-synonymous to synonymous polymorphism rates (pN/pS) will be calculated for each gene in each sample. A description of how the different population genomic parameters are calculated can be found [here](https://github.com/EnvGen/POGENOM/blob/master/POGENOM_parameter_calculations.pdf).

## Documentation ##
Documentation for POGENOM and the Input_POGENOM pipeline is hosted on [readthedocs](https://pogenom.readthedocs.org).

## Citing POGENOM ##
POGENOM doesn't have a paper yet, meanwhile please cite it like this:

Sjöqvist, Delgado Zambrano, Alneberg, Andersson AF (2020) POGENOM: population genomics from metagenomes https://github.com/EnvGen/POGENOM.

If you use the Input_POGENOM pipeline, please make sure to cite the software it depends on listed in the documentation.

