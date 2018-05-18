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
The *Your Analyses* page shows the collection of the uploaded files. 
The status column report the elaboration phase of the single analysis: analysing, analysed or error.
When the status correspont to *analysed*, the list of the annotated variants is available. 
With the folder icon, the user can to access to the *Variants analysis* page.
If the user wants to delete his analysis can use the trash icon.


Variants analysis
~~~~~~~~~~~~~~~~~

**Variants**

The *Variants* page shows the collection of the annotate VCF variants grouped under macro areas, as specified in :doc:`annotation`.

**Filter variants**

Through each of the column titles in the grid the user can easily add, edit or remove filters while reviewing the variants. 
Each filter that the user add through the column title will also be displayed in this pane on the left.

*...to be continued*

**Annotate variants**
To the left of each variant row there are three annotation types that can be defined per candidate variant. 
Clicking on this section will present the *Annotate variant* popup where it's possibile to define the relevance (High, Med or Low) and the pathogenicity of the variant on the top (Pathongenic, Likely Pathogenic, Uncertain Significance, Likely Benign, Benign). 
Below, it's possibile to add a note regarding the variant in free text.


Export filtered data
~~~~~~~~~~~~~~~~~~~~
Una volta filtrate le varianti è possibile esportare tutti i risultati visualizzati attraverso il bottone *Excel Export*.

