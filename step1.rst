.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


Sample dataset and preprocessing
-------------
In this tutorial, we are analyzing 1M reads from Arabidopsis thaliana leaf RNA-seq dataset (SRR7947123) from Zhao et al., 2018. Example data is available from CyVerse datastore.

----

**Input Data:**

.. list-table::
    :header-rows: 1

    * - Input
      - Description
      - Example
    * - Leaf RNA-seq data
      - 1M reads dataset from SRR7947123
      - iplantcollaborative > example_data > HAMR_tutorial -> fastqfiles

**Preprocessing**


*Evaluate the quality of your sequencing data using FastQC*

Preprocessing will assess the quality of the raw reads to identify possible sequencing errors or biases. FastQC can be used for an overview of the data quality.

1. Login to the |discovery_enviornment|.

2. Click on "Apps" tab in the Discovery Environment and search for "fastqc".

3. Click on the app icon.

4. Change the name of the analysis and output folder as needed or leave for defaults.

5. Under "Input" click on Add to provide input files. Sample dataset location iplantcollaborative > example_data > HAMR_tutorial -> fastqfiles. Check both files and click 'OK'. 

6. For next section "Resource Requirements" request resources as needed or leave for defaults 

7. Click **Launch Analysis**. You will receive a notification that the job has been submitted and running. Click on the Analyses tab to check the status of your job. When the analysis completes, click on the right three dots menu and click on 'Go to output folder' to access you output files.

**Output/Results**

.. list-table::
    :header-rows: 1

    * - Output
      - Description
      - Example
    * - html and zip files
      - FastqQC report
      - SRR7947123_1M_fastqc.html


----

**Description of output and results**

Click on the html report files and check if your sequencing data has any red flags that you should be aware of. For more details on each module of the fastqc report, check |fastqc_doc| 


----

**Fix or improve this documentation**

- Search for an answer:
  |CyVerse Learning Center|
- Ask us for help:
  click |Intercom| on the lower right-hand side of the page
- Report an issue or submit a change:
  |Github Repo Link|
- Send feedback: `learning@CyVerse.org <learning@CyVerse.org>`_

----

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

.. Comment: Place Images Below This Line
   use :width: to give a desired width for your image
   use :height: to give a desired height for your image
   replace the image name/location and URL if hyperlinked


 .. |Clickable hyperlinked image| image:: ./img/IMAGENAME.png
    :width: 500
    :height: 100
 .. _CyVerse logo: http://learning.cyverse.org/

 .. |Static image| image:: ./img/IMAGENAME.png
    :width: 25
    :height: 25



.. Comment: Place URLS Below This Line

   # Use this example to ensure that links open in new tabs, avoiding
   # forcing users to leave the document, and making it easy to update links
   # In a single place in this document

   .. |Substitution| raw:: html # Place this anywhere in the text you want a hyperlink

      <a href="REPLACE_THIS_WITH_URL" target="blank">Replace_with_text</a>


.. |Github Repo Link|  raw:: html

   <a href="https://github.com/CyVerse-learning-materials/HAMR-tutorial" target="blank">Github Repo Link</a>

.. |discovery_enviornment| raw:: html

    <a href="https://de.cyverse.org/de/" target="_blank">Discovery Environment</a>

.. |fastqc_app_icon| image:: ./img/fastqc.png
    :width: 300
    :height: 150
.. _fastqc_app_icon: http://learning.cyverse.org/ <a href="https://de.cyverse.org/de/" target="_blank">fastqc_app_icon</a>

.. |trim_app| raw:: html

    <a href="https://de.cyverse.org/de/?type=apps&app-id=92578d70-54b0-11e9-ae6e-008cfa5ae621&system-id=de" target="_blank">Trimmomatic app</a>


.. |fastqc_doc| raw:: html

    <a href="https://www.bioinformatics.babraham.ac.uk/projects/fastqc/Help/3%20Analysis%20Modules/" target="_blank">FastQC documentation</a>

.. |fastqc_tutorial| raw:: html

    <a href="https://cyverse-fastqc-quickstart.readthedocs-hosted.com/en/latest/" target="_blank">evaluate high-throughput sequencing reads with FastQC</a>
    
.. |trim_tutorial| raw:: html

    <a href="https://cyverse-trimmomatic-quickstart.readthedocs-hosted.com/en/latest/" target="_blank">here</a>
