# Test Directory Architecture
## test-dir-architecture
Proposals for re-architecturing the Genomics Test Directory for Rare Diseases (cancer may come later).

### Context
At present the [NHS England Genomics Test Directory](https://www.england.nhs.uk/publication/national-genomic-test-directories/) exists as a set of interlinked files:
1. **Eligibility criteria**: 
2. **Indication list**: the list of basic indications, R-numbers (test codes), specialty requesters, test methods etc.

Most of the panels refer to gene panels defined in the [NHS GMS section of panelapp](https://nhsgms-panelapp.genomicsengland.co.uk/).

The NHS GMS panels then refer back to the [main panelapp](https://panelapp.genomicsengland.co.uk/) area, where more detail on the review status of the panels is present, as well as phenotypes/conditions associated with the gene/panel.

## Issues
This architecture is somewhat fragmented, and this makes it difficult to navigate. It is also difficult for electronic systems such as Electronic Health Records (EHRs) and Order Communications systems (Ordercomms) to access the data to incorporate in patient care pathways.

## Solutions
Re-architecting of the Test Directory can solve a lot of these problems, making test request and result reporting easier.

- Phenotypes: HPO, OMIM, ORPHAnet etc
- Indications
- Eligibility & Appropriateness
- Clinical Decision Support
- Panels
- Genes
- Analytical modalities
- Registries
- Clinical pathways
- Research

This is a work in progress.

### We've started a [list of APIs](api_list.md) which we hope to add to soon, to start putting together a description of the required architecture.

