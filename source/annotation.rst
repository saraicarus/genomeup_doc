Variants annotation fields
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Location**
The position of variant as *chrom:start*. The *chrom* is the chromosome on which the variant resides (from VCF CHROM field) and *start* is the physical position on the chromosome (1-based coordinate).

**Gene**
The gene affected by the variant.



Genomic and genetic data
~~~~~~~~~~~~~~~~~~~~~~~~

**Ref**
Reference allele (from VCF REF field).

**Alt**
Alternate allele for the variant (from VCF ALT field).

**AA**
The amino acid change, when applicable in *ref-pos-alt* format. The '%3D' symbol results a deletion.

**Zygosity**
The zygosity of the variant in patient. Inferred from the VCF GT genotype tag as:  *het* for a call of a heterozygous genotype, *hom_ref* for a call of a homozygous reference genotype and *hom_alt* for a call of a homozygous alternate (variant) genotype.

**HGVS**
Human Genome Variation Sequence c-syntax nomenclature (from VEP).

**Genotype**
The sample genotypes.

**Genotype Depths**
The depth of aligned sequence observed for each sample.

**Genotype Quality**
the genotype quality (PHRED scale) estimates for each sample.

**RefSeq**
The transcripts (IDs) relevant to the effect on the protein.

**Codon**
What is the codon change?

**dbSNP**
A list of rs ids for variants present in dbSNP.



Variant Calling Q&R
~~~~~~~~~~~~~~~~~~~

**qual**
Variant confidence or quality by depth.

**depth**
The number of aligned sequence reads that led to this variant call.



Evidence
~~~~~~~~

**Clinvar Phenotypes**
‘,’ delimited list of phenotypes associated with this gene (includes any variant in the same gene in clinvar not just the current variant).

**Clinvar significance**
The clinical significance scores for each of the variant according to ClinVar: unknown, untested, non-pathogenic, probable-non-pathogenic,probable-pathogenic, pathogenic, drug-response, histocompatibility, other.

**COSMIC**
A list of known COSMIC ids for this variant.

**OMIM**

**MedGen**

**Orphanet**

**SNOMED**



Effect&Prediction
~~~~~~~~~~~~~~~~~

**Effect**
The consequence of the most severely affected transcript.

**Severity**
Severity of the highest order observed for the variant.

**GERP RS**
GERP conservation score (rejected substitution). Higher scores reflect greater conservation.

**LRT pred**
Prediction of our LR based ensemble prediction score, "T(olerated)" or "D(amaging)". The score cutoff between "D" and "T" is 0.5. The rankscore cutoff between "D" and "T" is 0.82268.

**MutTaster**
MutationTaster prediction.

**Polyphen2 HDIV**
Polyphen2 prediction based on HumDiv.

**Polyphen2 HVAR**
Polyphen2 prediction based on HumVar.

**SIFT**
SIFT predictions for the snp’s for the most severely affected transcript.


Frequency
~~~~~~~~~

**Max AF**
The maximum of  aaf_gnomad{afr,amr,eas,nfe,sas}, aaf_esp_ea, aaf_esp_aa, aaf_1kg_amr, aaf_1kg_eas, aaf_1kg_sas, aaf_1kg_afr, aaf_1kg_eur, aaf_adj_exac_afr, aaf_adj_exac_amr, aaf_adj_exac_eas, aaf_adj_exac_nfe, aaf_adj_exac_sas, and -1 if none of those databases/populations contain the variant.

**1K Genome AF**
Global allele frequency (based on AC/AN) (1000g project - phase 3)

**ESP African/American AF**
Minor Allele Frequency of the variant for African Americans in the ESP project

**ESP European/American AF**
Minor Allele Frequency of the variant for European Americans in the ESP project

**ExAC AF**
Raw allele frequency (population independent) of the variant based on ExAC exomes (AF)

**ExAC Het**
The number of heterozygote genotypes observed in ExAC. Pulled from the ExAC AC_Het INFO field.

**ExAC HOM**
The number of homozygous alt. genotypes observed in ExAC. Pulled from the ExAC AC_Het INFO field.

**ExAC EAS AF (%)**
Adjusted allele frequency (population independent) of the variant based on ExAC (Adj_AC/Adj_AN).


Proteomic and Proteic data
~~~~~~~~~~~~~~~~~~~~~~~~~~

**PDB**

**Domain**

**Topology**

**Open Target**

**Path. & Biotech**

**BIOMUTA**

**Exons**


GenomeUp Predictions
~~~~~~~~~~~~~~~~~~~~

**AI 2D**

**AI 3D**

**Homology Modeling**

**Docking**

**Molecular Dynamics**

**RMSD WTxMT**
