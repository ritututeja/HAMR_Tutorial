.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

Running HAMR
-------------

With the sorted, indexed, filtered for uniquely mapped and resolved for spliced alignment reads, HAMR tabulates the total number of high-quality mismatches at each candidate genomic site. HAMR then excludes the possibility that the observed mismatches are not due to sequencing error, SNP or RNA editing.

----

**Input Data:**

.. list-table::
    :header-rows: 1

    * - Input
      - Description
      - Example
    * - BAM file
      - BAM file with sorted, indexed, filtered for uniquely mapped and resolved for spliced alignment reads
      - iplantcollaborative > example_data > HAMR_tutorial -> resolved_splice_alignments

*RUN HAMR*

1. Click on "Apps" tab in the Discovery Environment and search for 'HAMR'.

2. Under Inputs section, provide input BAM file and reference genome. Leave prediction model file as default. 

3. Provide an output file and output prefix in outputs section or leave it to defaults.

4. Under parameters, provide min read quality= 30, min read cov= 10, seq error rate= 0.05, Hypothesis= H4, Max p-val= 0.01, Max FDR= 0.05, Max ref prec= 0.05 or change as desired.

5. Under optional parameters, indicate that the data is paired-end (pe) and filter-ends (fe). Filter-ends excludes the first and last positions in the read from the analysis. 


**Output/Results**

.. list-table::
    :header-rows: 1

    * - Output
      - Description
      - Example
    * - HAMR 
      - positions predicted to contain modified nucleotides
      - iplantcollaborative > example_data > HAMR_tutorial -> HAMR_output


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
