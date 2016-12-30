# multiplicom_brca

Pipeline for Multiplicom BRCA Tumor MASTR Dx sequenced with Illumina (MiSeq)

Command Example: ```. runBRCA.sh configuration.conf 161219-AR2DP_20161219_BRCA2 161219-AR2DP_20161219_BRCA2 1 1```

Tools used:
- FastQ Generation: bcl2fastq
- FastQ Trimming: FastX
- FastQ Quality Control: FastQC
- Alignment: BWA Mem
- Variant Calling: Samtools & Platypus
- Variant Filtering: VariantAnnotation
- Variant Annotation: Annotator

Settings for Variant Filtering
- Minimum Coverage: 500x
- Minimum Variant Allele Frequency: 5% (0.05)
- Strand Bias: 0
