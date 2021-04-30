# codon_rebalance

This python script uses hierarchical clustering to merge highly similar eccDNA forming regions together
Input format is currently hard coded and should be tab delimited file that looks like so:

## first row is header
## columns are Triplet, Amino Acid, Blank, Blank, Blank, Triplet, Fraction(yeast), Frequency(yeast), Number(yeast), Fraction(ecoli), Frequency(ecoli), Number(ecoli), Fraction(rice), Frequency(rice), Number(rice), Fraction(benthi), Frequency(benthi), Number(benthi)

Input arguments (in order)
## input table
## output name
## minimum fraction codon usage of other organism (not yeast) i.e. 0.1
## maximum fraction to remove of codon usage of yeast i.e. 0.3

# Example usage
## python3 ./rebalance_codon_usage.py codon_usage.tsv codon_usage_rebalanced.tsv 0.1 0.3
