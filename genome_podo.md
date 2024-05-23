# *Podospora anserina*'s genome

## Genome sequence



This is a fasta file that contains the whole genome sequence.

[Genome](genome_podo/genomePodoMatPlus.fasta)

This is a multifasta file with 7 fasta sequences corresponding to the 7 chromosomes.

We remind you that *P. anserina* as most fungi can have two mating types that control the sexual compatibility. In *P. anserina* there are called *mat*+ and *mat*-.
The sequenced strain was *mat*+, that's why the file name ends with "MatPlus".
The mating type locus is located on the 1st chromosome, that's why it's called Chr1plus in the fasta file.

You'll also find bellow 7 fasta files for the 7 chromosomes.

[Chromosome 1](genome_podo/chrm1plus.fasta)

[Chromosome 2](genome_podo/chrm2.fasta)

[Chromosome 3](genome_podo/chrm3.fasta)

[Chromosome 4](genome_podo/chrm4.fasta)

[Chromosome 5](genome_podo/chrm5.fasta)

[Chromosome 6](genome_podo/chrm6.fasta)

[Chromosome 7](genome_podo/chrm7.fasta)


## Annotation

Here is a gff file containing the genome annotation:

[Genome annotation](genome_podo/Annot_MatPlus2016_v2024-05.gff)

It contains coordinates and information about genes (TSS, TES, mRNAs), coding sequences (CDS), repeats, tRNA, centromeres etc.

Here are bed files with only selected annotation:
- [CDS](genome_podo/CDS-Merged_Podo_MatPlus_v3.bed) : contains the coordinates of CDSs (between START and STOP, regardless of introns)
- [Transcripts](genome_podo/Transcripts_Podo_MatPlus_v3.bed) : contains the coordinates of TSS and TES (only genes for which the prediction was possible)
- [Repeats](genome_podo/Repeat_Podo_MatPlus_v3.bed) : contains annotation of repeated sequences *i.e.* transposable elements and duplications

## Chromosome sizes

Here a file containing the size of each chromosome:

[Chromosome sizes](genome_podo/Chr_size.txt)


Some programs need this information.
