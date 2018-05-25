Getting started
^^^^^^^^^^^^^^^

GenomeUp allows to annotate, filter and view the variants of a .vcf file.
After the login, the user lands on a dashboard page called *Your Analyses*.
Into the *Your Analyses* page the user can explores its analyses and it can start a new analysis using our *Start a new analysis* wizard.
On the left, the user can finds the icon botton to return at home page, to start a new analysis, to read the user guide and to send us an email.

.. image :: /_static/your_analyses.jpg

Start a new analysis
~~~~~~~~~~~~~~~~~~~~
The user can begin a new analysis by clicking on the "Start a new analysis" button, in which a new sample can be uploaded (.vcf or .gz format) and, moreover, can be added other details about the subject.

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

.. image :: /_static/screen.png

**Variants**

The *Variants* page shows the collection of the annotated -vcf variants grouped by macro areas, as specified in :doc:`annotation`.

**Filter variants**

Through each of the column titles in the grid the user can easily add, edit or remove filters while reviewing the variants.
Clicking on the each colums titles the user can sort the data by ascending or discending order.

Furthermore, clicking on the rigth side of each columns titles, is avalaible a column menu with three panels: *filter tab*, *general tab* and *columns tab*.

.. image :: /_static/filter_tab.png

- **Filter tab**
    - Pin columns: to lock the specific column on right or left of table, above the other columns.
    - Autosize this column.
    - Autosize all columns.
    - Group by: to group by the content of the column.
    - Reset columns: to reset all filters and column setting.
    - Tool panel: to open the tool panel on right of table.
    
- **General tab**: to filter by content of the selected column. If the column content is alfhabetic will be appear the list of  content and a search tool for free text. If the column content is numerical will be appear different constraints: *equals, not equals, less than, less than or equals, greater than, greater than or equals,in range*.

- **Columns tab**: to show or hide column or group of columns.

On right of table is avalaible the tool pane.

.. image :: /_static/tool_panel.png

The **Tool panel** is split into difference sections which are follows:

- **Pivot mode section**: check the *Pivot Mode* checkbox to turn the grid into Pivot Mode. Pivoting allows the user to take a columns values and turn them into columns.
- **Column filter**: filter the column that the user wants show.
- **Columns section**: display all columns, grouped by column groups, that are available to be displayed in the grid. The order of the columns is the order in which columns were provided to the grid and do not change even if the user changes the column order inside the grid.
- **Row groups section**: columns here will form the grids row grouping. 
- **Values section**: columns here will When grouping, the user can apply an aggregation function to any column to populate the group row with values.

- **Side button**: shows and hides the tool panel.
- **Select/Unselect column**: each column can be individually selected. 
- **Drag handle**: each column can be dragged with the mouse. The column can then be dragged either to row groups section or to values section.


**Annotate variants**
Into the left of each variant row, there are three annotation types that can be defined per candidate variant.

.. image :: /_static/annotate_variants.png

Clicking Annotate variant to set the **relevance**: 
- High
- Med
- Low
and the **pathogenicity** of the variant:
- Pathogenic
- Likely Pathogenic
- Uncertain Significance
- Likely Benign
- Benign
Moreover, it’s possible to add a note using the textbox.

Export filtered data
~~~~~~~~~~~~~~~~~~~~
Once the variants are filtered, the user can download the report into an .xls file, by clicking on the *Excel Export* button.

