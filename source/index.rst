GenomeUp documentation
===============================

GenomeUp is a bioinformatics startup, based in Rome.
https://www.genomeup.com/


What we do
^^^^^^^^^^
The Whole Genomic Sequencing(WGS) data represents an opportunity, for doctors and patients, to draw personalized clinical therapies.

Currently, doctors are unable to exploit the full potential of the WGS data, for clinical purposes, without the assistance of bioinformaticians.

GenomeUP, through the development of their genomic tool, exploits the features of Artificial Intelligence (AI) bringing forward precision medicine, supporting doctors in drawing the treatment best fitting their patients’ needs.

On the basis of patients’ genome, doctors will be able to obtain a detailed clinical report on genes affecting patients’ pathology, the gravity of the new mutations selected and the latest personalized treatments found mining information from the world’s biggest biomedical database PubMed.

Integrating the genome knowledge and the translational medicine GenomeUP aims to improve patients’ treatments through the latest computer technologies.

The goal of GenomeUP is to equip doctors with all the information needed to understand the role the genome has in diseases and, also, to allow faster and more efficient diagnosis and treatments.

Variants annotation fields
^^^^^^^^^^^^^^^^^^^^^^^^^^
**General variant information**


*  **chrom**
The chromosome on which the variant resides (from VCF CHROM field).

*  **start(1-coor)**
Physical position on the chromosome as to hg19 (1-based coordinate)

*  **end**
The 1-based end position. (from VCF POS field, yet inferred based on the size of the variant)

*  **vcf_id**
The VCF IDfield.

*  **ref**
Reference allele (from VCF REF field).

*  **alt**
Alternate allele for the variant (from VCF ALT field).

*  **qual**
Quality score for the assertion made in ALT (from VCF QUAL field).

*  **filter**
A string of filters passed/failed in variant calling (from VCF FILTER field)

*  **type**
The type of variant  [snp, indel] .

*  **sub_type**
The variant sub-type. If type is snp: [ts, (transition), tv (transversion)]. If type is indel: [ins, (insertion), del (deletion)].

*  **vcf_id**
The VCF IDfield.

*  **anno_id**
Variant transcript number for the most severely affected transcript [capire se serve]

**Structural variation columns**

*  **sv_cipos_start_left**
The leftmost position of the leftmost SV breakpoint confidence interval.

*  **sv_cipos_end_left**
The rightmost position of the leftmost SV breakpoint confidence interval.

*  **sv_cipos_start_right**
The leftmost position of the rightmost SV breakpoint confidence interval.

*  **sv_cipos_end_right**
The rightmost position of the rightmost SV breakpoint confidence interval.

*  **sv_length**
The length of the structural variant in base pairs.

*  **sv_is_precise**
Is the structural variant precise (i.e., to 1-bp resolution)?

*  **sv_tool**
The name of the SV discovery tool used to find the SV.

*  **sv_evidence_type**
What type of alignment evidence supports the SV?

*  **sv_event_id**
A unique identifier for the SV.

*  **sv_mate_id**  
The ID for the “other end” of the SV.

*  **sv_strand**
The orientations of the SV breakpoint(s).

**call_rate**
The fraction of samples with a valid genotype.

**NCBI information**
*  **in_dbsnp**
Absence (0) or presence (1) of the variant in dbsnp

*  **rs_ids**
A comma-separated list of rs ids for variants present in dbSNP

**Clinical information**
*  **clinvar_sig**
The clinical significance scores for each of the variant according to ClinVar: unknown, untested, non-pathogenic, probable-non-pathogenic,probable-pathogenic, pathogenic, drug-response, histocompatibility, other

*  **clinvar_disease_name**
The name of the disease to which the variant is relevant

*  **clinvar_dbsource**
Variant Clinical Channel IDs

*  **clinvar_dbsource_id**
The record id in the above database

*  **clinvar_origin** 
The type of variant: unknown, germline, somatic, inherited, paternal, maternal, de-novo, biparental, uniparental, not-tested, tested-inconclusive, other

*  **clinvar_dsdb**
Variant disease database name

*  **clinvar_dsdbid**
Variant disease database ID

*  **clinvar_disease_acc** 
Variant Accession and Versions

*  **clinvar_in_locus_spec_db**
Submitted from a locus-specific database?

*  **clinvar_on_diag_assay**
Variation is interrogated in a clinical diagnostic assay?

*  **clinvar_causal_allele** 
The allele(s) that are associated or causal for the disease.

*  **clinvar_gene_phenotype**
‘,’ delimited list of phenotypes associated with this gene (includes any variant in the same gene in clinvar not just the current variant).

*  **in_omim**
Absence (0) or presence (1) of the variant in OMIM database

**uniprot_acc**
Uniprot accession number. Multiple entries separated by ";"

**uniprot_id**
Uniprot ID number. Multiple entries separated by ";"

**uniprot_aapos**
Amino acid position as to Uniprot. Multiple entries separated by ";"

**geno2mp_hpo_ct**
Value from geno2mp indicating count of HPO profiles. Set to -1 if missing

**pfam_domain**
Pfam protein domain that the variant affects

**interpro_domain**
Domain annotations come from Interpro database. The number in the brackets following a specific domain is the count of times Interpro assigns the variant position to that domain, typically coming from different predicting databases. Multiple entries separated by ";".

**fold_degenerate**
Degenerate type (0, 2 or 3)

**cyto_band**
Chromosomal cytobands that a variant overlaps

**rmsk**
A comma-separated list of RepeatMasker annotations that the variant overlaps. Each hit is of the form: name_class_family

**in_cpg_island**
Does the variant overlap a CpG island?. Based on UCSC: Regulation > CpG Islands > cpgIslandExt

**in_segdup**
Does the variant overlap a segmental duplication?. Based on UCSC: Variation&Repeats > Segmental Dups > genomicSuperDups track

**is_conserved**
Does the variant overlap a conserved region? Based on the 29-way mammalian conservation study.

**gerp_bp_score**
GERP conservation score. Higher scores reflect greater conservation. At base-pair resolution.

**gerp_element_pval**
GERP elements P-val. Lower P-values scores reflect greater conservation. Not at base-pair resolution.

**num_hom_ref**
The total number of of homozygotes for the reference (ref) allele

**num_het**
The total number of heterozygotes observed.

**num_hom_alt**
The total number of homozygotes for the reference (alt) allele

**num_unknown**
The total number of unknown genotypes

**aaf**
The observed allele frequency for the alternate allele

**hwe**
The Chi-square probability of deviation from HWE (assumes random mating)

**inbreeding_coeff**
The inbreeding co-efficient that expresses the likelihood of effects due to inbreeding

**pi**
The computed nucleotide diversity (pi) for the site

**recomb_rate**
Returns the mean recombination rate at the variant site. Based on HapMapII_GRCh37 genetic map

**gene**
Corresponding gene name of the highly affected transcript

**transcript**
The variant transcript that was most severely affected. (for two equally affected transcripts, the protein_coding biotype is prioritized (SnpEff/VEP)

**is_exonic** 
Does the variant affect an exon for >= 1 transcript?

**is_coding**
Does the variant fall in a coding region (excl. 3’ & 5’ UTRs) for >= 1 transcript?

**is_splicing**
Does the variant affect a canonical or possible splice site? That is, set to TRUE if the SO term is any of splice_acceptor_variant, splice_donor_variant, or splice_region_variant.

**is_lof** 
Based on the value of the impact col, is the variant LOF for >= transcript?

**exon**
Exon information for the severely affected transcript

**aaf**
The observed allele frequency for the alternate allele

**codon_change**
What is the codon change?

**aa_change**
What is the amino acid change (for a snp)?

**aa_length**
Has the format pos/len when biotype=protein_coding, is empty otherwise. len=protein length. pos = position of the amino acid change when is_coding=1 and is_exonic=1, ‘-‘ otherwise.

**aaalt**  
Alternative amino acid. "." if the variant is a splicing site SNP (2bp on each end of an intron)

**aaref**
Reference amino acid. "." if the variant is a splicing site SNP (2bp on each end of an intron)

**aapos_SIFT**
ENSP id and amino acid positions corresponding to SIFT scores. Multiple entries separated by ";"

**aapos_FATHMM**
ENSP id and amino acid positions corresponding to FATHMM scores. Multiple entries separated by ";"

**biotype**
The ‘type’ of the severely affected transcript (e.g., protein-coding, pseudogene, rRNA etc.) (only SnpEff)

**impact**
The consequence of the most severely affected transcript

**impact_so**
The Sequence ontology term for the most severe consequence

**impact_severity** 
Severity of the highest order observed for the variant

**Function predictor**

*  **Polyphen2_HDIV_score_dbNSFP**
Polyphen2 score based on HumDiv, i.e. hdiv_prob. The score ranges from 0 to 1. Multiple entries separated by ";"

*  **Polyphen2_HDIV_rankscore_dbNSFP**
Polyphen2 HDIV scores were first ranked among all HDIV scores in dbNSFP. The rankscore is the ratio of the rank the score over the total number of the scores in dbNSFP. If there are multiple scores, only the most damaging (largest) rankscore is presented. The scores range from 0.02656 to 0.89917

*  **Polyphen2_HDIV_pred_dbNSFP**
Polyphen2 prediction based on HumDiv

*  **Polyphen2_HVAR_score_dbNSFP**
Polyphen2 score based on HumVar, i.e. hvar_prob. The score ranges from 0 to 1. Multiple entries separated by ";"

*  **Polyphen2_HVAR_rankscore_dbNSFP**
Polyphen2 HVAR scores were first ranked among all HVAR scores in dbNSFP. The rankscore is the ratio of the rank the score over the total number of the scores in dbNSFP. If there are multiple scores, only the most damaging (largest) rankscore is presented. The scores range from 0.01281 to 0.9711

*  **Polyphen2_HVAR_pred_dbNSFP**
Polyphen2 prediction based on HumVar

*  **sift_pred**
SIFT predictions for the snp’s for the most severely affected transcript (only VEP)

*  **sift_score**
SIFT scores for the predictions (only VEP)

*  **SIFT_score_dbNSFP**
SIFT score (SIFTori). Scores range from 0 to 1. The smaller the score the more likely the SNP has damaging effect. Multiple scores separated by ";"

*  **SIFT_pred_dbNSFP** 
If SIFTori is smaller than 0.05 (rankscore>0.55) the corresponding non-synonymous SNP is predicted as "D(amaging)"; otherwise it is predicted as "T(olerated)". Multiple predictions separated by ";"

*  **SIFT_converted_rankscore_dbNSFP**
SIFTori scores were first converted to SIFTnew=1-SIFTori, then ranked among all SIFTnew scores in dbNSFP. The rankscore is the ratio of the rank the SIFTnew score over the total number of SIFTnew scores in dbNSFP. If there are multiple scores, only the most damaging (largest) rankscore is presented. The rankscores range from 0.02654 to 0.87932

*  **LRT_score**
Our logistic regression (LR) based ensemble prediction score, which incorporated 10 scores (SIFT, PolyPhen-2 HDIV, PolyPhen-2 HVAR, GERP++, MutationTaster, Mutation Assessor, FATHMM, LRT, SiPhy, PhyloP) and the maximum frequency observed in the 1000 genomes populations. Larger value means the SNV is more likely to be damaging. Scores range from 0 to 1

*  **LRT_rankscore**
LR scores were ranked among all LR scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of LR scores in dbNSFP. The scores range from 0 to 1

*  **LRT_pred**
Prediction of our LR based ensemble prediction score, "T(olerated)" or "D(amaging)". The score cutoff between "D" and "T" is 0.5. The rankscore cutoff between "D" and "T" is 0.82268

*  **MutationAssessor_score** 
MutationAssessor functional impact combined score (MAori)

*  **MutationAssessor_rankscore**
MAori scores were ranked among all MAori scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of MAori scores in dbNSFP. The scores range from 0 to 1

*  **MutationAssessor_pred** 
MutationAssessor's functional impact of a variant

*  **MutationTaster_score** 
MutationTaster p-value (MTori), ranges from 0 to 1

*  **MutationTaster_converted_rankscore** 
The MTori scores were first converted: if the prediction is "A" or "D" MTnew=MTori; if the prediction is "N" or "P", MTnew=1-MTori. Then MTnew scores were ranked among all MTnew scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of MTnew scores in dbNSFP. The scores range from 0.0931 to 0.80722

*  **MutationTaster_pred**
MutationTaster prediction

*  **FATHMM_score** 
FATHMM default score (FATHMMori)

*  **FATHMM_rankscore** 
FATHMMori scores were ranked among all FATHMMori scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of FATHMMori scores in dbNSFP. If there are multiple scores, only the most damaging (largest) rankscore is presented. The scores range from 0 to 1

*  **FATHMM_pred** 
If a FATHMM_score is <=-1.5 (or rankscore <=0.81415) the corresponding non-synonymous SNP is predicted as "D(AMAGING)"; otherwise it is predicted as "T(OLERATED)". Multiple predictions separated by ";"

*  **MetaSVM_score** 
Our support vector machine (SVM) based ensemble prediction score, which incorporated 10 scores (SIFT, PolyPhen-2 HDIV, PolyPhen-2 HVAR, GERP++, MutationTaster, Mutation Assessor, FATHMM, LRT, SiPhy, PhyloP) and the maximum frequency observed in the 1000 genomes populations. Larger value means the SNV is more likely to be damaging.
Scores range from -2 to 3 in dbNSFP

*  **MetaSVM_rankscore**
MetaSVM scores were ranked among all MetaSVM scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of MetaSVM
scores in dbNSFP. The scores range from 0 to 1.

*  **MetaSVM_pred**  
Prediction of our SVM (radial kernel support vector) machine based ensemble prediction score, "T(olerated)" or "D(amaging)". The score cutoff between "D" and "T" is 0. The rankscore cutoff between "D" and "T" is 0.83357

*  **MetaLR_score** 
Our logistic regression (LR) based ensemble prediction score, which incorporated 10 scores (SIFT, PolyPhen-2 HDIV, PolyPhen-2 HVAR, GERP++, MutationTaster, Mutation Assessor, FATHMM, LRT, SiPhy, PhyloP) and the maximum frequency observed in the 1000 genomes populations. Larger value means the SNV is more likely to be damaging. Scores range from 0 to 1

*  **MetaLR_rankscore**
LR scores were ranked among all LR scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of LR scores in dbNSFP. The scores range from 0 to 1

*  **MetaLR_pred** 
Prediction of our LR based ensemble prediction score, "T(olerated)" or "D(amaging)". The score cutoff between "D" and "T" is 0.5. The rankscore cutoff between "D" and "T" is 0.82268

*  **VEST3_score** 
VEST 3.0 score. Score ranges from 0 to 1. The larger the score the more likely the mutation may cause functional change. Multiple scores separated by ";", corresponding to Transcript_id_VEST3. Please note this score is free for non-commercial use. For more details please refer to http://wiki.chasmsoftware.org/index.php/SoftwareLicense.

*  **VEST3_rankscore** 
VEST3 scores were ranked among all VEST3 scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of VEST3 scores in dbNSFP. In case there are multiple scores for the same variant, the largest score (most damaging) is presented. The scores range from 0 to 1. 

*  **VEST3_pred**
Variant Effect Scoring Tool version 3 prediction.

*  **PROVEAN_score**
Protein Variation Effect Analyzer with clustering of homologus  sequences method. Scores range from -14 to 14. The smaller the score the more likely the SNP has damaging effect. 

*  **PROVEAN_converted_rankscore**
PROVEANori were first converted to PROVEANnew=1-(PROVEANori+14)/28, then ranked among all PROVEANnew scores in dbNSFP. The rankscore is the ratio of the rank the PROVEANnew score over the total number of PROVEANnew scores in dbNSFP. If there are multiple scores, only the most damaging (largest) rankscore is presented.
The scores range from 0 to 1.

*  **PROVEAN_pred** 
If PROVEANori <= -2.5 (rankscore>=0.543) the corresponding nsSNV is predicted as "D(amaging)"; otherwise it is predicted as "N(eutral)". Multiple predictions separated by ";", corresponding to Ensembl_proteinid.

*  **Reliability_index**
Number of observed component scores (except the maximum frequency in the 1000 genomes populations) for RadialSVM and LR. Ranges from 1 to 10. As RadialSVM and LR scores are calculated based on imputed data, the less missing component scores, the higher the reliability of the scores and predictions

*  **LRT_Omega**
Estimated nonsynonymous-to-synonymous-rate ratio (Omega, reported by LRT)

**Conservation scores**

*  **CADD_raw_dbNSFP** 
Combined annotation dependent depletion prediction: higher values are more deleterious.

*  **CADD_raw_rankscore_dbNSFP**
CADD raw scores were ranked among all CADD raw scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of CADD raw scores in dbNSFP. 

*  **CADD_phred_dbNSFP** 
CADD phred-like score. This is phred-like rank score based on whole genome CADD raw scores.

*  **GERPpp_NR**
GERP++ neutral rate

*  **GERPpp_RS**
GERP++ RS score, the larger the score, the more conserved the site

*  **GERPpp_RS_rankscore**
GERP++ RS scores were ranked among all GERP++ RS scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of GERP++ RS scores in dbNSFP

*  **phyloP46way_primate**
phyloP (phylogenetic p-values) conservation score based on the multiple alignments of 10 primate genomes (including human). The larger the score, the more conserved the site

*  **phyloP46way_primate_rankscore**
phyloP46way_primate scores were ranked among all phyloP46way_primate scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of phyloP46way_primate scores in dbNSFP

*  **phyloP46way_placental**
phyloP (phylogenetic p-values) conservation score based on the multiple alignments of 33 placental mammal genomes (including human). The larger the score, the more conserved the site

*  **phyloP46way_placental_rankscore**
phyloP46way_placental scores were ranked among all phyloP46way_placental scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of phyloP46way_placental scores in dbNSFP

*  **phyloP100way_vertebrate**
phyloP (phylogenetic p-values) conservation score based on the multiple alignments of 100 vertebrate genomes (including human). The larger the score, the more conserved the site

*  **phyloP100way_vertebrate_rankscore**
phyloP100way_vertebrate scores were ranked among all phyloP100way_vertebrate scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of phyloP100way_vertebrate scores in dbNSFP

*  **phastConsP46way_primate**
phyloP (phylogenetic p-values) conservation score based on the multiple alignments of 10 primate genomes (including human). The larger the score, the more conserved the site

*  **phastConsP46way_primate_rankscore**
phyloP46way_primate scores were ranked among all phyloP46way_primate scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of phyloP46way_primate scores in dbNSFP

*  **phastConsP46way_placental** 
phastCons conservation score based on the multiple alignments of 33 placental mammal genomes (including human). The larger the score, the more conserved the site

*  **phastConsP46way_placental_rankscore**
phastCons46way_placental scores were ranked among all phastCons46way_placental scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of phastCons46way_placental scores in dbNSFP

*  **phastConsP100way_vertebrate**
phastCons conservation score based on the multiple alignments of 100 vertebrate genomes (including human). The larger the score, the more conserved the site

*  **phastConsP100way_vertebrate_rankscore**
phastCons100way_vertebrate scores were ranked among all phastCons100way_vertebrate scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of phastCons100way_vertebrate scores in dbNSFP

*  **SiPhy_29way_pi** 
The estimated stationary distribution of A, C, G and T at the site, using SiPhy algorithm based on 29 mammals genomes

*  **SiPhy_29way_logOdds**
SiPhy score based on 29 mammals genomes. The larger the score, the more conserved the site

*  **SiPhy_29way_logOdds_rankscore**
SiPhy_29way_logOdds scores were ranked among all SiPhy_29way_logOdds scores in dbNSFP. The rankscore is the ratio of the rank of the score over the total number of SiPhy_29way_logOdds scores in dbNSFP

*  **fitcons**
fitCons scores estimating the probability that a point mutation at each position in a genome will influence fitness. Higher scores have more potential for interesting genomic function. Common ranges: 0.05-0.35 for non-coding and 0.4-0.8 for coding

**UniSNP_ids**
rs numbers from UniSNP, which is a cleaned version of dbSNP build 129, in format: rs number1;rs number2;...

**ancestral_allele**
Ancestral allele (based on 1000 genomes reference data)

**rms_bq** 
The RMS base quality at this position.

**cigar** 
CIGAR string describing how to align an alternate allele to the reference allele.
depth
The number of aligned sequence reads that led to this variant call

**strand_bias**
Strand bias at the variant position. From the “SB” tag.

**rms_map_qual**
RMS mapping quality, a measure of variance of quality scores

**in_hom_run**
Homopolymer runs for the variant allele

**num_mapq_zero**
Total counts of reads with mapping quality equal to zero

**num_alleles** 
Total number of alleles in called genotypes

**num_reads_w_dels**
Fraction of reads with spanning deletions

**haplotype_score**
Consistency of the site with two segregating haplotypes

**qual_depth**
Variant confidence or quality by depth

**allele_count** 
Allele counts in genotypes

**allele_bal** 
Allele balance for hets

**in_hm2**
Whether the variant was part of HapMap2.

**in_hm3**
Whether the variant was part of HapMap3.

**is_somatic** 
Whether the variant is somatically acquired.

**somatic_score**
A score for 

**in_esp**
Presence/absence of the variant in the ESP project data

**exome_chip**
Whether a SNP is on the Illumina HumanExome Chip

**Population information**

*  **max_aaf_all**
The maximum of aaf_gnomad{afr,amr,eas,nfe,sas},aaf_esp_ea, aaf_esp_aa, aaf_1kg_amr, aaf_1kg_eas,aaf_1kg_sas,aaf_1kg_afr,aaf_1kg_eur,aaf_adj_exac_afr,aaf_adj_exac_amr,aaf_adj_exac_eas,aaf_adj_exac_nfe,aaf_adj_exac_sas. and -1 if none of those databases/populations contain the variant.

*  **aaf_esp_ea**
Minor Allele Frequency of the variant for European Americans in the ESP project

*  **aaf_esp_aa**
Minor Allele Frequency of the variant for African Americans in the ESP project

*  **aaf_esp_all** 
Minor Allele Frequency of the variant w.r.t both groups in the ESP project

*  **in_1kg**
Presence/absence of the variant in the 1000 genome project data (phase 3)

*  **aaf_1kg_amr**
Allele frequency of the variant in AMR population based on AC/AN (1000g project, phase 3)

*  **aaf_1kg_eas**
Allele frequency of the variant in EAS population based on AC/AN (1000g project, phase 3)

*  **aaf_1kg_sas**
Allele frequency of the variant in SAS population based on AC/AN (1000g project, phase 3)

*  **aaf_1kg_afr** 
Allele frequency of the variant in AFR population based on AC/AN (1000g project, phase 3)

*  **aaf_1kg_eur** 
Allele frequency of the variant in EUR population based on AC/AN (1000g project, phase 3)

*  **aaf_1kg_all** 
Global allele frequency (based on AC/AN) (1000g project - phase 3)

*  **ARIC5606_AA_AC**
Alternative allele counts in 2403 exomes of African Americans from the Atherosclerosis Risk in Communities Study (ARIC) cohort study.

*  **ARIC5606_AA_AF**
Alternative allele frequency of 2403 exomes of African Americans from the Atherosclerosis Risk in Communities Study (ARIC) cohort study.

*  **ARIC5606_EA_AC**
Alternative allele counts in 3203 exomes of European Americans from the Atherosclerosis Risk in Communities Study (ARIC) cohort study.

*  **ARIC5606_EA_AF**
Alternative allele frequency of 3203 exomes of European Americans from the Atherosclerosis Risk in Communities Study (ARIC) cohort study.

*  **in_exac**
Presence/absence of the variant in ExAC (Exome Aggregation Consortium) data (Broad)

*  **aaf_exac_all**
Raw allele frequency (population independent) of the variant based on ExAC exomes (AF)

*  **aaf_adj_exac_all**
Adjusted allele frequency (population independent) of the variant based on ExAC (Adj_AC/Adj_AN)

*  **aaf_adj_exac_afr**
Adjusted allele frequency of the variant for AFR population in ExAC (AC_AFR/AN_AFR)

*  **aaf_adj_exac_amr**
Adjusted allele frequency of the variant for AMR population in ExAC (AC_AMR/AN_AMR)

*  **aaf_adj_exac_eas**
Adjusted allele frequency of the variant for EAS population in ExAC (AC_EAS/AN_EAS)

*  **aaf_adj_exac_fin**
Adjusted allele frequency of the variant for FIN population in ExAC (AC_FIN/AN_FIN)

*  **aaf_adj_exac_nfe**
Adjusted allele frequency of the variant for NFE population in ExAC (AC_NFE/AN_NFE)

*  **aaf_adj_exac_oth**
Adjusted allele frequency of the variant for OTH population in ExAC (AC_OTH/AN_OTH)

*  **aaf_adj_exac_sas**
Adjusted allele frequency of the variant for SAS population in ExAC (AC_SAS/AN_SAS)

*  **exac_num_het**
The number of heterozygote genotypes observed in ExAC. Pulled from the ExAC AC_Het INFO field.

*  **exac_num_hom_alt** 
The number of homozygous alt. genotypes observed in ExAC. Pulled from the ExAC AC_Het INFO field.

*  **exac_num_chroms**
The number of chromosomes underlying the ExAC variant call. Pulled from the ExAC AN_Adj INFO field.

*  **aaf_gnomad_all**
Allele frequency (population independent) of the variant in gnomad

*  **aaf_gnomad_afr**
Allele frequency (AFR population) of the variant in gnomad

*  **aaf_gnomad_amr**
Allele frequency (AMR population) of the variant in gnomad

*  **aaf_gnomad_asj**
Allele frequency (ASJ population) of the variant in gnomad

*  **aaf_gnomad_eas**
Allele frequency (EAS population) of the variant in gnomad

*  **aaf_gnomad_fin**
Allele frequency (FIN population) of the variant in gnomad

*  **aaf_gnomad_nfe**
Allele frequency (NFE population) of the variant in gnomad

*  **aaf_gnomad_oth**
Allele frequency (OTH population) of the variant in gnomad

*  **aaf_gnomad_sas**
Allele frequency (SAS population) of the variant in gnomad

*  **gnomad_num_het**
Number of het genotypes observed in gnomad

*  **gnomad_num_hom_alt**
Number of hom_alt genotypes observed in gnomad

*  **gnomad_num_chroms**
Number of chromosomes genotyped in gnomad

**grc**
Association with patch and fix regions from the Genome Reference Consortium: http://www.ncbi.nlm.nih.gov/projects/genome/assembly/grc/human/ Identifies potential problem regions associated with variant calls.

**gms_illumina**
Genome Mappability Scores (GMS) for Illumina error models. Provides low GMS scores (< 25.0 in any technology) from: http://sourceforge.net/apps/mediawiki/gma-bio/index.php?title=Download_GMS

**gms_solid**
Genome Mappability Scores with SOLiD error models

**gms_iontorrent**
Genome Mappability Scores with IonTorrent error models

**in_cse**
Is a variant in an error prone genomic position, using CSE: Context-Specific Sequencing Errors

**vista_enhancers**
Experimentally validated human enhancers from VISTA (http://enhancer.lbl.gov/frnt_page_n.shtml)

**ENCODE information**

*  **encode_tfbs**
Comma-separated list of transcription factors that were observed by ENCODE to bind DNA in this region. Each hit in the list is constructed as TF_CELLCOUNT, where: TF is the transcription factor name, CELLCOUNT is the number of cells tested that had nonzero signals.

*  **encode_dnaseI_cell_count**
Count of cell types that were observed to have DnaseI hypersensitivity.

*  **encode_dnaseI_cell_list** 
Comma separated list of cell types that were observed to have DnaseI hypersensitivity. Provenance: Thurman, et al, Nature, 489, pp. 75-82, 5 Sep. 2012

*  **encode_consensus_gm12878**
ENCODE consensus segmentation prediction for GM12878. CTCF: CTCF-enriched element; E: Predicted enhancer; PF: Predicted promoter flanking region; R: Predicted repressed or low-activity region; TSS: Predicted promoter region including TSS; T: Predicted transcribed region; WE: Predicted weak enhancer or open chromatin cis-regulatory element | unknown: This region of the genome had no functional prediction.

*  **encode_consensus_h1hesc**
ENCODE consensus segmentation prediction for h1HESC.

*  **encode_consensus_helas3**
ENCODE consensus segmentation prediction for Helas3.

*  **encode_consensus_hepg2**
ENCODE consensus segmentation prediction for HEPG2.

*  **encode_consensus_huvec**
ENCODE consensus segmentation prediction for HuVEC.

*  **encode_consensus_k562**
ENCODE consensus segmentation prediction for k562.


**Cancer related columns**

*  **COSMIC_ID**
A list of known COSMIC ids for this variant.

*  **COSMIC_CNT**
The count of known COSMIC ids for this variant.


**HGVS nomenclature**
*  **vep_hgvsc**
Human Genome Variation Sequence c-syntax nomenclature (from VEP)

*  **vep_hgvsp**
Human Genome Variation Sequence p-syntax nomenclature (from VEP)

*  **vep_hgvs_offset**
Human Genome Variation Sequence nomenclature offset(from VEP)

.. toctree::
   :maxdepth: 2

   contact


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
