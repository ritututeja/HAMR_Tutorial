.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_


Filter multi-mapping reads and add read groups
-----------------------------------------------

HAMR requires that reads map unambiguously to a reference sequence, in order to avoid false-positive mismatches. Workflow-extractUniqueReads, retains uniquely mapping reads and converts to the sorted BAM format. Next step *resolving spliced alignments using GATK* requires assigning reads in a file to a read-group. Picard AddorReplaceGroups DE app will be used for assignment of read-group.

----

**Input Data:**

.. list-table::
    :header-rows: 1

    * - Input
      - Description
      - Example
    * - HISAT2 output file
      - Alignment file in BAM format
      - iplantcollaborative > example_data > HAMR_tutorial -> mapped_reads

**RUN Workflow-extractUniqueReads**


1. Click on "Apps" tab in the Discovery Environment and search for "Workflow-extractUniqueReads".

2. Click on the app icon and change the name of the analysis and output folder as desired.

3. Under Step1- Samtools 1.11 BAM to SAM provide input BAM file from the data store. Example data for this step is provided at iplantcollaborative > example_data > HAMR_tutorial -> mapped_reads -> SRR7947123_1M_1.sorted.bam. In the next step, getuniquereads provide the output file name and click Launch Analysis.

**RUN Picard AddorReplaceReadGroups**

1. Search for the app "Picard" in Apps search window.

2. Click on the app icon 'Picard AddorReplaceReadGroups v2.5'.

3. Under the Inputs section provide the output from the Workflow-extractUniqueReads. Example data is provided at iplantcollaborative > example_data > HAMR_tutorial -> unique_mapping_reads -> output_sorted.bam. Provide Read group ID, library, platform, platform unit and sample name.

4. Under output section, provide the output file name and click Launch Analysis.

**Output/Results**

.. list-table::
    :header-rows: 1

    * - Output
      - Description
      - Example
    * - Assigned read groups
      - BAM file with assigned read groups
      - iplantcollaborative > example_data > HAMR_tutorial -> unique_mapping_reads_assignRG -> output.RG.bam


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
