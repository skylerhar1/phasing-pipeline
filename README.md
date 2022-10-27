# phasing-pipeline
process of using whatshap phasing
Reference genome
1: index reference genome
2: map raw reads to reference genome to get bam files
3: create a vcf file from the illumina bam files
4: whatshap phase with vcf file, and all bam files

Low coverage genomes
1: index reference genome
2: map raw reads to reference genome to create lots of bam files
3: create many gvcf files
4: merge gvcf files
5: merge bam files
(make sure read groups stay intact @RG)
6: index bam files
7: run whatshap script
