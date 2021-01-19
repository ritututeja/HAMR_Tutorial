.. include:: cyverse_rst_defined_substitutions.txt
.. include:: custom_urls.txt

|CyVerse_logo|_

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`_

**HAMR Tutorial**
=================

..
High Throughput Annotation of Modified Ribonucleotides (HAMR) detects modified ribonucleotides based upon their ability to intefere with Watson-Crick base pairing. This leads to reverse transcriptase base misincorporations, which can be detected as mismatches from the reference genome in cDNA-based RNA-seq libraries. HAMR tabulates these mismatches and tests for patterns of mismatches that cannot be explained by: Sequencing errors, Single nucleotide polymorphisms (SNPs) or RNA editing.

In this tutorial, we will be using Cyverse Discovery Environment (DE) public apps for analysis of a sample dataset. Command-line expertise is not required to follow most of this tutorial.

Tutorial Maintainer(s)
------------------------

Who to contact if this guide needs fixing. You can also email
`learning@CyVerse.org <learning@CyVerse.org>`_

.. list-table::
    :header-rows: 1

    * - Maintainer
      - Institution
      - Contact
    * - Reetu Tuteja
      - CyVerse / UA
      - reetututeja@cyverse.org
----

.. toctree::
	:maxdepth: 2

	Sample dataset and preprocessing <step1.rst>
  Read mapping <step2.rst>
  Filter multi-mapping reads and add read groups <step3.rst>
  Resolve spliced alignments using GATK <step4.rst>
  Running HAMR <step5.rst>
  Further reading <step6.rst>


Prerequisites
-------------

Downloads, access, and services
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*In order to complete this tutorial you will need access to the following services/software*

..
	#### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Prerequisite
      - Preparation/Notes
      - Link/Download
    * - CyVerse account
      - You will need a CyVerse account to complete this exercise
      - |CyVerse User Portal|

Platform(s)
~~~~~~~~~~~

*We will use the following CyVerse platform(s):*

 ..
   #### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Platform
      - Interface
      - Link
      - Platform Tour
    * - Data Store
      - GUI/Command line
      - |Data Store|
      - |Data Store Guide|
    * - Discovery Environment
      - Web/Point-and-click
      - |Discovery Environment|
      - |Discovery Environment Guide|

Application(s) used
~~~~~~~~~~~~~~~~~~~
..
	#### Comment: these tables are examples, delete whatever is unnecessary ####

**Discovery Environment App(s):**

.. list-table::
    :header-rows: 1

    * - App name
      - Version
      - Description
      - App link
      - Notes/other links
    * - Muscle
      - 3.8.31
      - Multiple sequence aligner
      -	|CyVerse_launch|
      - |Original App Documentation|
    * - HiSAT2-index-align-2.1
      - 3.8.31
      - Short-reads sequence aligner
      - |CyVerse_launch|
      - |Original App Documentation|
    * - Workflow-extractUniqueReads
      - Samtools 1.11
      - |CyVerse_launch|
      - |Original App Documentation|
    * - Picard
      - 2.8
      - |CyVerse_launch|
      - |Original App Documentation|
    * - GATK
      - 3.5
      - |CyVerse_launch|
      - |Original App Documentation|
    * - HAMR
      - HAMR 1.11
      - |CyVerse_launch|
      - |Original App Documentation|


Input and example data
~~~~~~~~~~~~~~~~~~~~~~

*In order to complete this tutorial you will need to have the following inputs prepared*

..
	#### comment: delete any row not needed in this table ####

.. list-table::
    :header-rows: 1

    * - Input File(s)
      - Format
      - Preparation/Notes
      - Example Data
    * -
      -
      -
      -

----

**Fix or improve this documentation**

- Search for an answer:
  |CyVerse Learning Center|
- Ask us for help:
  click |Intercom| on the lower right-hand side of the page
- Report an issue or submit a change:
  |Github Repo Link|
- Send feedback: `learning@CyVerse.org <learning@CyVerse.org>`_

.. comment:

   Uncomment the below and fix with this repo's information if citing

   **Citation**

   You may cite this work as:
   [Repository Title]
   [Author(s)]
   [Repository Release Version]
   [DOI: Zenodo DOI link (generated from Github Release/Zenodo)]
----

|Home_Icon|_
`Learning Center Home <http://learning.cyverse.org/>`__


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

.. |Download Cyberduck| raw:: html

   <a href="https://cyberduck.io/" target="blank">Download Cyberduck</a>

.. |Original App Documentation|  raw:: html

   <a href="http://www.drive5.com/muscle/manual/" target="blank">Original App Documentation</a>
