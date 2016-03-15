# PharmacotherapyDB: `catalog` contents

This directory contains the following files:

+ [`indications.tsv`](indications.tsv) contains drug–disease pairs and their consensus category (`DM`, `SYM`, or `NOT`). `n_curators` refers to how many of the three curators initially assigned the consensus classification. `n_resources` refers to how many of the four resources (MEDI-HPS, LabeledIn, EHRLink, PREDICT) included the indication.

+ [`diseases.tsv`](diseases.tsv) contains a list of diseases with indications. For each disease, the number of indications per category is provided.

+ [`drugs.tsv`](drugs.tsv) contains a list of drugs with indications. For each drug, the number of indications per category is provided.

+ [`catalog.xlsx`](catalog.xlsx) is a spreadsheet with four sheets:

  1. `indications` — data from `indications.tsv`
  2. `diseases` — data from `diseases.tsv`
  3. `drugs` — data from `drugs.tsv`
  4. `curation` — the classifications from each of the three physician curators (`AJG`, `CSH`, & `PK`).

If you have any questions, feel free to create [an issue](https://github.com/dhimmel/indications/issues "GitHub Issues for dhimmel/indications").
