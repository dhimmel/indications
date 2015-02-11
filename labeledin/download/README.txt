===========================================================================
*
*                            PUBLIC DOMAIN NOTICE
*               National Center for Biotechnology Information
*
*  This software/database is a "United States Government Work" under the
*  terms of the United States Copyright Act.  It was written as part of
*  the author's official duties as a United States Government employee and
*  thus cannot be copyrighted.  This software/database is freely available
*  to the public for use. The National Library of Medicine and the U.S.
*  Government have not placed any restriction on its use or reproduction.
*
*  Although all reasonable efforts have been taken to ensure the accuracy
*  and reliability of the software and data, the NLM and the U.S.
*  Government do not and cannot warrant the performance or results that
*  may be obtained by using this software or data. The NLM and the U.S.
*  Government disclaim all warranties, express or implied, including
*  warranties of performance, merchantability or fitness for any 
*  particular purpose.
*
*  Please cite the authors in any work or product based on this material.
*  1. Khare R, Li J, Lu Z. LabeledIn: cataloging labeled indications for human 
*     drugs. J Biomed Inform. 2014 Dec;52:448-56. 
*
*  2. Khare R, Wei CH, Lu Z. Automatic Extraction of Drug Indications from 
*     FDA Drug Labels. AMIA Annu Symp Proc. 2014
* 
*  3. Khare R, Li J, Lu Z. Toward Creating a Gold Standard of Drug Indications 
*     from FDA Drug Labels.in Proceedings of the IEEE International Conference 
*     on Healthcare Informatics (ICHI) 2013, Philadelphia USA. Sept 9-11, 2013
*
*
==========================================================================

LabeledIn DATASET (Released September 04 2014)
==========================================================================

GENERAL DESCRIPTION
--------------------------------------------------------------------------
LabeledIn contains annotations of drug indications in FDA drug labels 
(DailyMed Version: August 28, 2012). LabeledIn is available in 3 formats: 

(1) Annotated XML format 
(2) Structured format 
(3) Visual HTML format. 

This release contains the LabeledIn dataset and the annotation guidelines. 

==========================================================================
CONTENTS
--------------------------------------------------------------------------
#1. Project Overview
--------------------------------------------------------------------------
Highlights of LabeledIn are presented in LabeledIn Overview Slides.pdf

--------------------------------------------------------------------------
#2. Annotated XML Format
--------------------------------------------------------------------------
LabeledIn_annotated_XML.txt contains the drug labels and in-text 
annotations formatted in XML. Each line corresponds to an annotated drug 
label; the pipe-delimited fields represent the following information:
  i.   study_drug_label_ID: The internal id for a drug label in our study
  ii.  DailyMed_SPL_ID: The unique drug label id (Set ID) in DailyMed        
  iii. indication section (with expert annotations): This field contains
       the INDICATIONS and USAGE section extracted from the drug label. 
       The specific indication mentions in the text are highlighted using 
       XML tags (<annotation>)represented the annotated mentions and the 
       corresponding disease identifier (attribute cui) in the UMLS
  iv.  Other_DailyMed_SPL_ID(s): the  DailyMed Set ID corresponding to 
       other drug labels that are similar to this drug label

--------------------------------------------------------------------------
#3. Structured Format
--------------------------------------------------------------------------
LabeledIn_Structured_Results.txt is a pipe-delimited file containing:
  i.   study_drug_label_ID: The internal id for a drug label in our study 
  ii.  DailyMed_SPL_ID: The  unique drug label ID (Set ID) in DailyMed
  iii. UMLS_CUI(s): The UMLS concept ID(s) for the annotated indication(s) 
  iv.  IN_RXCUI: The linked RxNorm ID for ingredient 
  v.   SCDF_RXCUI: The linked RxNorm ID for ingredient+doseform 
  vi.  SCD_RXCUI: The linked RxNorm ID for ingredient+doseform+strength
  vii. Other_SCDF_RXCUI: The linked RxNorm ID for the ingredient+doseform        
       of other similar drug labels
  viii.Other_SCD_RXCUI: The linked RxNorm ID for the 
       ingredient+doseform+strength of other similar drug labels

--------------------------------------------------------------------------
#4. Visual HTML Format
--------------------------------------------------------------------------
This format contains the LabeledIn_corpus.html file that visually presents 
the information contains in the other two formats. 

--------------------------------------------------------------------------
#5. Annotation Guidelines
--------------------------------------------------------------------------
Annotation_Guidelines.pdf contains guidelines for annotating LabeledIn. 


