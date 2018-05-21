Getting started
^^^^^^^^^^^^^^^

GenomeUp allows to annotate, filter and view the variants of a .vcf file.
After the login, the user lands on a dashboard page called *Your Analyses*.
Into the *Your Analyses* page the user can explores its analyses and it can start a new analysis using our *Start a new analysis* wizard.
On the left, the user can finds the icon botton to return at home page, to start a new analysis, to read the user guide and to send us an email.

.. image :: /_static/your_analyses.jpg

Start a new analysis
~~~~~~~~~~~~~~~~~~~~
The user can begin a new analysis by clicking on the "Start a new analysis" button, in which a new sample can be uploaded (.vcf format) and, moreover, can be added other details about the subject.

.. image :: /_static/start_new_analysis.jpg


**Subject** *(required)*
Set the name of the analysis. 

**Reference Genome** *(required)*
Choose the version of the `reference <https://en.wikipedia.org/wiki/Reference_genome>`_ assembled sequence database of the human genome: GRCh37(or hg19) and GRCh38.

**Gender** *(optional)*
Set the gender of patient of the sample. 

**Ethnicity** *(optional)*
Set the population type in: African/African American (AFR), Latino (AMR), Ashkenazi Jewish (ASJ), East Asian (EAS), Finnish (FIN), Non-Finnish European (NFE), South Asian (SAS), Other (OTH).

**Phenotype** *(optional)*
Specify the phenotype under consideration following the `HPO <http://human-phenotype-ontology.github.io/>`_ format.

Analyses
~~~~~~~~
The *Your Analyses* page shows the collection of the uploaded files. 
The field *status* shows the elaboration phase of the single analysis: analysing, analysed or error.
When the status switch into *analysed*, the list of the annotated variants is available. 
With the folder icon, the user can to access to the *Variants analysis* page.
If the user wants to delete one of its analysis can use the trash icon.


Variants analysis
~~~~~~~~~~~~~~~~~

**Variants**

The *Variants* page shows the collection of the annotated -vcf variants grouped by macro areas, as specified in :doc:`annotation`.

**Filter variants**

Through each of the column titles in the grid the user can easily add, edit or remove filters while reviewing the variants. 

*...to be continued*

**Annotate variants**
Into the left of each variant row there are three annotation types that can be defined per candidate variant. 
Clicking on this section will appear the *Annotate variant* popup where it's possibile to set the relevance (High, Med or Low) and the pathogenicity of the variant on the top (Pathongenic, Likely Pathogenic, Uncertain Significance, Likely Benign, Benign). 
Motreover, it's possibile to add a note using the textbox.


Export filtered data
~~~~~~~~~~~~~~~~~~~~
Once filtered the variants, the user can export into an .xls fine through the *Excel Export* bottun.

