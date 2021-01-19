.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


Resolve spliced alignments using GATK
--------------------------------------
In this step, we will process BAM files from previous step to resolve splice alignments. GATK is strict about chromosome order, and thus we include preventative re-sorting steps using Picard-ReorderSAM app. 

----

**Input Data:**

.. list-table::
    :header-rows: 1

    * - Input
      - Description
      - Example
    * - BAM files
      - BAM files with uniquely mapped reads
      - iplantcollaborative > example_data > HAMR_tutorial -> unique_mapping_reads_assignRG -> output.RG.bam

**RUN Picard-ReorderSAM**

1. Click on "Apps" tab in the Discovery Environment and search for "Picard-ReorderSAM".

2. Under Input section, provide input BAM file (output from Picard-AddOrReplaceReadGroups). Provide Reference sequence, dictionary and index files from the tutorial example data (iplantcollaborative > example_data > HAMR_tutorial -> reference_genome). Reference dict for your genome can be generated using GATK-CreateSequenceDictionary app.

3. Provide an output file name or leave it to defaults and launch analysis.

**Splits reads that contain Ns in their cigar string using GATK-SplitNCigarReads**

1. Search for "GATK-SplitNCigarReads v3.5" from the app tab. Click on the app icon.

2. Provide Reference sequence, dictionary and index files from the tutorial example data. Input reordered BAM and index file from the previous step. Example data for this step is provided at iplantcollaborative > example_data > HAMR_tutorial -> reordered_BAM_files.

3. Provide an output file name or leave it to defaults and launch analysis.


**Output/Results**

.. list-table::
    :header-rows: 1

    * - Output
      - Description
      - Example
    * - BAM file
      - BAM file with reads split at N CIGAR elements and CIGAR strings updated.
      - iplantcollaborative > example_data > HAMR_tutorial -> resolved_splice_alignments

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
