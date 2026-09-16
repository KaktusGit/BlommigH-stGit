## Format exercise findings

### FASTQ
```bash
$ zcat reads.fastq.gz | wc -l | awk '{print $1/4}'
```
* **Number of reads:** 1000
* **Are all reads of the same length?:** No
* **Quality encoding:** Phred+33
* **Notes:** 

### GTF/GFF
* **Number of genes:** 37184
* **Most exon-dense gene:**
  ```text
  99 Potra2n15c28530
  94 Potra2n4c10448
  92 Potra2n17c31702
  84 Potra2n3c6871
  84 Potra2n19c34342
  ```


### BAM
* **Number of mapped reads:** 51073157
* **% of properly paired reads:** 48300964 + 0 properly paired (95.35% : N/A)
* **Number of reference sequences:**
  ```bash
  \$ samtools view -H alignment.bam > header.txt ; grep -c "@SQ" header.txt
  ```
  *Resultat:* 1601


### VCF
* **Total variants:** 78358
* **Variants in Potra2n1c1:** 130
* **SNPs / indels:** 56197
