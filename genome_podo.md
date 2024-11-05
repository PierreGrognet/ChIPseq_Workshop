# *Podospora anserina*'s genome

## Genome sequence



This is a fasta file that contains the whole genome sequence: [Genome](genome_podo/genomePodoMatPlus.fasta)

This is a multifasta file with 7 fasta sequences corresponding to the 7 chromosomes.

We remind you that, as most fungi, *P. anserina* can have two mating types that control the sexual compatibility. In *P. anserina* there are called *mat*+ and *mat*-.
The sequenced strain was *mat*+, that's why the file name ends with "MatPlus".
The mating type locus is located on the 1st chromosome, that's why it's called Chr1plus in the fasta file.

You'll also find bellow the 7 individual fasta files for the 7 chromosomes.

* [Chromosome 1](genome_podo/chrm1plus.fasta)
* [Chromosome 2](genome_podo/chrm2.fasta)
* [Chromosome 3](genome_podo/chrm3.fasta)
* [Chromosome 4](genome_podo/chrm4.fasta)
* [Chromosome 5](genome_podo/chrm5.fasta)
* [Chromosome 6](genome_podo/chrm6.fasta)
* [Chromosome 7](genome_podo/chrm7.fasta)


## Annotations

#### Here is a gff file containing the genome annotation:

[Genome annotation](genome_podo/Annot_MatPlus2016_v2024-10.gff)

It contains coordinates and information about genes (TSS, TES, mRNAs), exons, coding exons (labeled as CDS), repeats, tRNA, centromeres etc. This file can be uploaded on IGV.


#### Below are BED files with only selected annotations:

- [CDS](genome_podo/CDS-Merged_Podo_MatPlus_v3.bed) : contains the coordinates of CDSs (between START and STOP, regardless of introns)
- [Transcription units](genome_podo/Transcripts_Podo_MatPlus_v3.bed) : constains the coordinates or the transcripts (mRNA)
- [Transcriptions sites](genome_podo/Transcription_sites_Podo_MatPlus_v3.bed) : contains the coordinates of TSS and TES (only for a subset of the genes for which the prediction was possible)
- [Repeats](genome_podo/Repeat_Podo_MatPlus_v3.bed) : contains the coordinates of repeated sequences *i.e.* transposable elements and duplications

These files contain coordinates and strand information for diverse genomic features. This file can be uploaded on IGV. They will be needed to run ``deeptools computeMatrix`` over these elements.


#### Below is a gff file containing the CDS only:
[CDS annotation](genome_podo/CDS-Merged_Podo_MatPlus_v3.gff)

## Chromosome sizes

Here a file containing the size of each chromosome:

[Chromosome sizes](genome_podo/Chr_size.txt)


Some programs need this information.
