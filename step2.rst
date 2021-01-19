.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


**Read mapping**
------------------

In this step, we will align our reads to the A. thaliana (TAIR10) reference genome. We will be using HiSAT2-index-align app from the Discovery Environment (DE) that builds a HISAT2 index for your genome and then map the reads.

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
    * - Reference Genome
      - A. thaliana TAIR 10 assembly
      - iplantcollaborative > example_data > HAMR_tutorial -> reference_genome

**Run HISAT2 in the CyVerse Discovery Environment**

1. Click on "Apps" tab in the Discovery Environment and search for "hisat2".

2. Click on the app icon HISAT2-index-align-2.1. 

3. Change the name of the analysis and output folder as needed or leave for defaults.

4. Under Input section provide Reference genome file in Fasta format. Browse through the datastore and provide TAIR10_allchr.fasta reference genome. This file is provided with the sample dataset- iplantcollaborative > example_data > HAMR_tutorial -> reference_genome.

5. Provide FASTQ files from the path iplantcollaborative > example_data > HAMR_tutorial -> fastqfiles. Choose the File type as PE for this dataset and click launch analysis.


**Output/Results**

.. list-table::
    :header-rows: 1

    * - Output
      - Description
      - Example
    * - Alignment files
      - Alignment files in BAM format
      - SRR7947123_1M.sorted.bam

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

   <a href="FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX_FIX" target="blank">Github Repo Link</a>
