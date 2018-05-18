Getting started
^^^^^^^^^^^^^^^

GenomeUp allow to annotate, filter and visualize the variants of a VCF file.
After the login, the user landing on a dashboard paga called *Your Analyses*.
Into the *Your Analyses* page the user can explors his analyses and allows to start a new analysis using our *Start a new analysis* wizard.
On left, the user can finds the icon botton to return at home page, to start new analysis, read the user guide and contacts form.

.. image :: /_static/your_analyses.jpg

Start new analysis
~~~~~~~~~~~~~~~~~~
The user can initiate a new analysis by clicking on the "Start a new analysis" button, which in a new samples can be uploaded (VCF format) and other details regarding the subject of the analysis can be entered.

.. image :: /_static/start_new_analysis.jpg


**Subject** *(required)*
Set the name of the analysis. 

**Reference Genome** *(required)*
Version of the `reference <https://en.wikipedia.org/wiki/Reference_genome/>`_ assembly database to the genome alignment: GRCh37(or hg19) and GRCh38.

**Gender** *(optional)*
Set the gender of patient of the sample. 

**Ethnicity** *(optional)*
Set the population type in: African/African American (AFR), Latino (AMR), Ashkenazi Jewish (ASJ), East Asian (EAS), Finnish (FIN), Non-Finnish European (NFE), South Asian (SAS), Other (OTH).

**Phenotype** *(optional)*
To specify the phenotype under consideration. Consider to follow the `HPO <http://human-phenotype-ontology.github.io/>`_ format.

Analyses
~~~~~~~~


Variants analysis
~~~~~~~~~~~~~~~~~
After the VCF file upload, it'll possible see the new analysis into *Analyses* page with the status field on working mode.
Dopo un po' di tempo, nel momento in cui lo status dell'analisi passa ad è possibile esplorare le varianti annotate clikando sull'icona [folder].

**Variants**

The *Variants* page shows the collection of the annotate VCF variants grouped under macro areas, as specified in :doc:`annotation`.

**Filter variants**

Filtrare le varianti è possibile attraverso diversi strumenti di filtraggio.
Ogni campo di annotazione è ordinabile secondo valori crescenti o decrescenti semplicemente clickando sull'header della colonna.

*...to be continued*

**Annotate variants**
To the left of each variant row there are three annotation types that can be defined per candidate variant. 
Clicking on this section will present the *Annotate variant* popup where it's possibile to define the relevance (High, Med or Low) and the pathogenicity of the variant on the top (Pathongenic, Likely Pathogenic, Uncertain Significance, Likely Benign, Benign). 
Below, it's possibile to add a note regarding the variant in free text.


Export filtered data
~~~~~~~~~~~~~~~~~~~~
Una volta filtrate le varianti è possibile esportare tutti i risultati visualizzati attraverso il bottone *Excel Export*.

