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
*  warranties of performance, merchantability or fitness for any particular
*  purpose.
*  
*  Please cite the authors in any work or product based on this material.
*  1. Khare R et al., Scaling drug indication curation through crowdsourcing,
*  Database, 2015 
*
===========================================================================

CROWDSOURCING DRUG INDICATION DATASET (Released January 31 2015)
===========================================================================

GENERAL DESCRIPTION
---------------------------------------------------------------------------
This dataset contains the crowdsourced annotations of drug indications in 
FDA drug labels (DailyMed Version: August 28, 2012).   

===========================================================================


CONTENTS
---------------------------------------------------------------------------
#1. New HITs - Structured Format 
(Total 3004 HITs corresponding to 706 DailyMed Drug Labels)
---------------------------------------------------------------------------
Crowdsourced_Results.txt is a pipe-delimited file containing:
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
  ix.  Crowdsourced answer by Majority voting (i.e. indication or not)

---------------------------------------------------------------------------
#2. answer codes
---------------------------------------------------------------------------
The file answer_codes.txt contains the descriptions of various answer codes 
listed in the last field of Crowdsourced_Results.txt
