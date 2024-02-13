# Resilience AI Augmented Systemic Literature Review

## Data Collection

### Crossref

Search query: https://api.crossref.org/works?query=resilient+resilience+resiliency&filter=has-abstract:true,type:journal-article&cursor=* 

- 'resilient' or 'resilience' or resiliency' must appear in both the title and abstract

### Scopus

Search query: https://api.elsevier.com/content/search/scopus?query=title(resiliency OR resilient OR resilience)&view=COMPLETE&cursor=*&count=25

- 'resilient' or 'resilience' or resiliency' must appear in both the title and abstract

### OpenAlex (in-progress)

## Cleaning

- Removed Journal Article Tag Suite (JATS) notation from the abstracts, if present
- Eliminated records with duplicate DOIs (first observation kept)
- Eliminated records with duplicate abstracts (first observation kept)
- Eliminated records with abstracts not detected to be in English via [langdetect](https://pypi.org/project/
