Getting started
^^^^^^^^^^^^^^^

GenomeUp allow to annotate, filter and visualize the variants of a VCF file.


Start new analysis
~~~~~~~~~~~~~~~~~~
The first operation is the upload of a VCF analysis file. 
After login, you can use the bottom called "Start a new analysis" to upload a VCF file.

.. image :: /_static/start_new_analysis.png


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

Export data
~~~~~~~~~~~
Una volta filtrate le varianti è possibile esportare tutti i risultati visualizzati attraverso il bottone *Excel Export*.

