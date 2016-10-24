class: center, middle

# FISH 546 
## Bioinformatics for Environmental Sciences

https://github.com/sr320/course-fish546-2016/wiki

##genefish.info

Steven Roberts
@sr320

---

## Reminders

- We will not going through manuals 

- 



---

class: center, middle


# RNA-Seq


---

## Transcriptome Assembly

- All the genes (expressed)!

--

- Necessary for de novo (no genome) expression analysis

--

- Memory intensive

--

- Primary software - Trinity


---

## Trinity

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Home_·_trinityrnaseq_trinityrnaseq_Wiki_1DBE50A5.png" alt="Home_·_trinityrnaseq_trinityrnaseq_Wiki_1DBE50A5.png"/>


---


<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Accessing_Trinity_on_Publicly_Available_Compute_Resources_·_trinityrnaseq_trinityrnaseq_Wiki_1DBE5204.png" alt="Accessing_Trinity_on_Publicly_Available_Compute_Resources_·_trinityrnaseq_trinityrnaseq_Wiki_1DBE5204.png"/>

---

## Example code

```
Trinity.pl
--seqType fq
--JM 24G
--left /Volumes/web/cnidarian/Geo_Pool_F_GGCTAC_L006_R1_001_val_1.fq /Volumes/web/cnidarian/Geo_Pool_M_CTTGTA_L006_R1_001_val_1.fq
--right /Volumes/web/cnidarian/Geo_Pool_F_GGCTAC_L006_R2_001_val_2.fq /Volumes/web/cnidarian/Geo_Pool_M_CTTGTA_L006_R2_001_val_2.fq
--CPU 16
```

---

## Evaluating assembly

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Transrate_-_transcriptome_assembly_quality_analysis_1DBE53AF.png" alt="Transrate_-_transcriptome_assembly_quality_analysis_1DBE53AF.png"/>


---

## Overview

Transrate analyses a transcriptome assembly in three key ways:

--

- by inspecting the contig sequences

--

- by mapping reads to the contigs and inspecting the alignments

--

- by aligning the contigs against proteins or transcripts from a related species and inspecting the alignments

---

## Lots you can do "within Trinity"

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Trinity_Transcript_Quantification_·_trinityrnaseq_trinityrnaseq_Wiki_1DBE5496.png" alt="Trinity_Transcript_Quantification_·_trinityrnaseq_trinityrnaseq_Wiki_1DBE5496.png"/>


---

## Basic


### Get Counts - do stats



---

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Screenshot_10_24_16__8_19_AM_1DBE5DFC.png" alt="Screenshot_10_24_16__8_19_AM_1DBE5DFC.png"/>





---

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Screenshot_10_24_16__8_12_AM_1DBE5C48.png" alt="Screenshot_10_24_16__8_12_AM_1DBE5C48.png"/>

### Example running DESeq2 

<https://github.com/sr320/eimd-sswd/blob/master/eimd_analysis.ipynb>





---

# With Genome...

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/TopHat_1DBE5B6E.png" alt="TopHat_1DBE5B6E.png"/>


---

## Example

Within Cyverse

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Screenshot_10_24_16__8_10_AM_1DBE5C07.png" alt="Screenshot_10_24_16__8_10_AM_1DBE5C07.png"/>

<https://github.com/sr320/course-fish546-2015/blob/master/notebooks/Sam_RNA-seq.ipynb>

---





