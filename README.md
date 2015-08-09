# Parsing Indication Databases

Here, we parse and compare several indications resources. See the following Thinklab discussions for more information:

+ [How should we construct a catalog of drug indications?](http://thinklab.com/discussion/how-should-we-construct-a-catalog-of-drug-indications/21)

See the `data` directory for merged datasets combining the following resources.

## LabeledIn

See [`labeledin`](labeledin) and [this Thinklab discussion](http://thinklab.com/discussion/processing-labeledin-to-extract-indications/46) for parsing the [data](http://ftp.ncbi.nlm.nih.gov/pub/lu/LabeledIn/) from:

> Khare R, Li J, Lu Z (2014) **LabeledIn: Cataloging labeled indications for human drugs**. *Journal of Biomedical Informatics* DOI: [10.1016/j.jbi.2014.08.004](https://dx.doi.org/10.1016/j.jbi.2014.08.004)

> Khare R, Burger JD, Aberdeen JS,Tresner-Kirsch DW, Corrales TJ, Hirchman L, Lu Z (2015) **Scaling drug indication curation through crowdsourcing**. *Database* DOI: [10.1093/database/bav016](https://dx.doi.org/10.1093/database/bav016)

Also see the [analysis notebook](http://git.dhimmel.com/indications/labeledin/) for visualization.

## MEDI

See [`medi`](medi) and [this Thinklab discussion](http://thinklab.com/discussion/medi-indications-data-discrepancy-in-resource-specific-counts/31) for parsing the [data](http://knowledgemap.mc.vanderbilt.edu/research/content/MEDI) from:

> Wei WQ, Cronin RM, Xu H, Lasko TA, Bastarache L, Denny JC (2013) **Development and evaluation of an ensemble resource linking medications to their indications.** *Journal of the American Medical Informatics Association* DOI: [10.1136/amiajnl-2012-001431](http://dx.doi.org/10.1136/amiajnl-2012-001431)

Also see the [analysis notebook](http://git.dhimmel.com/indications/medi/) for visualization.

## ehrlink

See [`ehrlink`](ehrlink) and [this Thinklab discussion](http://thinklab.com/discussion/extracting-indications-from-the-ehrlink-resource/62) for parsing data from ehrlink:

> McCoy AB et al. (2012) **Development and evaluation of a crowdsourcing methodology for knowledge base construction: identifying relationships between clinical problems and medications** *Journal of the American Medical Informatics Association* DOI: [10.1136/amiajnl-2012-000852](https://dx.doi.org/10.1136/amiajnl-2012-000852)

## PREDICT

See [`msb-predict`](msb-predict) for parsing data from PREDICT:

> Gottlieb A, Stein GY, Ruppin E, Sharan R (2011) **PREDICT: a method for inferring novel drug indications with application to personalized medicine.** *Molecular Systems Biology*. DOI: [10.1038/msb.2011.26](https://dx.doi.org/10.1038/msb.2011.26)

## SIDER

SIDER is not directly included here but may be of interest. SIDER 4 has been parsed in a [seperate respository](https://github.com/dhimmel/SIDER4). SIDER 2 has been parsed in a [seperate respository](https://github.com/dhimmel/SIDER2) and corresponding [web tutorial](http://git.dhimmel.com/SIDER2/).

