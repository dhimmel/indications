# PharmacotherapyDB: the Open Catalog of Drug Therapies for Disease

PharmacotherapyDB is a catalog of medical indications between small molecule compounds and complex human diseases. We created the resource as part of our network-based drug repurposing project. However, PharmacotherapyDB is designed to be broadly applicable as a gold standard of drug indications for computational approaches. The catalog adheres to pathophysiological principals first. Therefore, the catalog includes indications with a poor risk–benefit ratio that are rarely used in the modern clinic.

PharmacotherapyDB differentiates between disease-modifying and symptomatic treatments. Each indication has been reviewed by multiple physicians. We use standardized vocabularies (the [Disease Ontology](http://disease-ontology.org/) and [DrugBank](http://www.drugbank.ca/)) to facilitate data integration.

Indications were classified by physician curators into three categories:

+ `DM` -- disease modifying
+ `SYM` -- symptomatic
+ `NOT` -- non-indication

This **initial release** contains 97 diseases and 601 drugs. Between these drug–disease pairs, there are 755 disease-modifying therapies, 390 symptomatic therapies, and 243 non-indications. Read more about the initial release [on Thinklab](http://doi.org/10.15363/thinklab.d182). The catalog data is available in [`catalog`](catalog) and on [figshare](https://doi.org/10.6084/m9.figshare.3103054).

## Data Integration

We [combined four resources](https://doi.org/10.15363/thinklab.d21#21) to create a high-confidence set of indications. See the `data` directory for merged datasets combining the following resources.

+ **LabeledIn**: See [`labeledin`](labeledin), [Thinklab](https://doi.org/10.15363/thinklab.d46), and [this notebook](http://git.dhimmel.com/indications/labeledin/) for parsing the [data](http://ftp.ncbi.nlm.nih.gov/pub/lu/LabeledIn/) from:

  > Khare R, Li J, Lu Z (2014) **LabeledIn: Cataloging labeled indications for human drugs**. *Journal of Biomedical Informatics* DOI: [10.1016/j.jbi.2014.08.004](https://doi.org/10.1016/j.jbi.2014.08.004)

  > Khare R, Burger JD, Aberdeen JS,Tresner-Kirsch DW, Corrales TJ, Hirchman L, Lu Z (2015) **Scaling drug indication curation through crowdsourcing**. *Database* DOI: [10.1093/database/bav016](https://doi.org/10.1093/database/bav016)

+ **MEDI**: See [`medi`](medi) and [this Thinklab discussion](https://doi.org/10.15363/thinklab.d31) for parsing the [data](http://knowledgemap.mc.vanderbilt.edu/research/content/MEDI) from:

  > Wei WQ, Cronin RM, Xu H, Lasko TA, Bastarache L, Denny JC (2013) **Development and evaluation of an ensemble resource linking medications to their indications.** *Journal of the American Medical Informatics Association* DOI: [10.1136/amiajnl-2012-001431](https://doi.org/10.1136/amiajnl-2012-001431)

  Also see the [analysis notebook](http://git.dhimmel.com/indications/medi/) for visualization.

+ **EHRLink**: See [`ehrlink`](ehrlink) and [this Thinklab discussion](https://dx.doi.org/10.15363/thinklab.d62) for parsing data from ehrlink:

  > McCoy AB et al. (2012) **Development and evaluation of a crowdsourcing methodology for knowledge base construction: identifying relationships between clinical problems and medications** *Journal of the American Medical Informatics Association* DOI: [10.1136/amiajnl-2012-000852](https://doi.org/10.1136/amiajnl-2012-000852)

+ **PREDICT**: See [`msb-predict`](msb-predict) for parsing data from PREDICT:

  > Gottlieb A, Stein GY, Ruppin E, Sharan R (2011) **PREDICT: a method for inferring novel drug indications with application to personalized medicine.** *Molecular Systems Biology*. DOI: [10.1038/msb.2011.26](https://doi.org/10.1038/msb.2011.26)

+ **SIDER** is not directly included here but may be of interest. SIDER 4 has been parsed in a [seperate respository](https://github.com/dhimmel/SIDER4). SIDER 2 has been parsed in a [seperate respository](https://github.com/dhimmel/SIDER2) and corresponding [web tutorial](http://git.dhimmel.com/SIDER2/).

## Curation

Three [physicians curated](https://doi.org/10.15363/thinklab.d95) the catalog to classify indications according to the three categories (`DM`, `SYM`, `NOT`). See [`curation`](curation) for this analysis.

## License

All original content in this repository is released under [CC0](https://creativecommons.org/publicdomain/zero/1.0/). Please also abide by the licenses of the sources if using their data. The Disease Ontology is released under [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/). DrugBank [requires permission](https://github.com/dhimmel/integrate/blob/145810796f0729d1ed5255bcb83c658490a198f9/licenses/custom/DrugBank.md) for commercial reuse. LabaledIn data is [public domain](https://github.com/dhimmel/integrate/blob/145810796f0729d1ed5255bcb83c658490a198f9/licenses/custom/LabeledIn.txt). MEDI and PREDICT data are [CC BY-NC-SA 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US). EHRLink data was [retrieved from](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3422843/#__sec21title) PubMed Central and does not specify a license.

**Disclaimer**: The repository is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the repository or the use or other dealings in the repository.
