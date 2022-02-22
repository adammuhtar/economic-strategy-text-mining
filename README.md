
# Text mining analysis of the UK's economic strategies

This repository provides data and notebooks with accompanying documentation to replicate the text mining analysis in the article "You’re not speaking my language: policy discontinuity and implementation gaps in the UK’s place-based economic strategies" (forthcoming). (please acknowledge if using the codes).

## Data
This study mines and analyses text to measure the take-up of policies announced under the 2017 Industrial Strategy, 2021 Plan for Growth and 2021 Innovation Strategy, on a sample of 85 policy documents and reports produced by the following ministerial departments or agencies:
* [British Business Bank (BBB)](https://www.british-business-bank.co.uk/)
* [British Patient Capital (BPC)](https://www.britishpatientcapital.co.uk/)
* [UK Export Finance (UKEF)](https://www.gov.uk/government/organisations/uk-export-finance)
* [UK Government Investments (UKGI)](https://www.ukgi.org.uk/)
* [The Cabinet Office](https://www.gov.uk/government/organisations/cabinet-office)
* [Department for Digital, Culture, Media and Sport (DCMS)](https://www.gov.uk/government/organisations/department-for-digital-culture-media-sport)
* [Department for Environment, Food & Rural Affairs (DEFRA)](https://www.gov.uk/government/organisations/department-for-environment-food-rural-affairs)
* [Department for Education (DfE)](https://www.gov.uk/government/organisations/department-for-education)
* [Department for Transport (DfT)](https://www.gov.uk/government/organisations/department-for-education)
* [Department of Health and Social Care (DHSC)](https://www.gov.uk/government/organisations/department-of-health-and-social-care)
* [Department for International Trade (DIT)](https://www.gov.uk/government/organisations/department-for-international-trade)
* [Ministry of Defence (MoD)](https://www.gov.uk/government/organisations/ministry-of-defence)

Text extraction is done using the [PyMuPDF](https://pymupdf.readthedocs.io/en/latest/) package and stored in `doc/text_extracted`.

## Code
This repository uses Python code to process the data. That code can be found in the following notebook:

### [`uk_economic_strategy_text_mining_analysis.ipynb`](notebook/uk_economic_strategy_text_mining_analysis.ipynb)

- Defines dictionary of search terms and term frequency function based on conditions (variations on spelling, case sensitivity, abbreviations, duplications, etc.).
- Merges term frequency counts based on publications and publishing institutions.
- Manually curated information needed to produce term frequency heatmaps.
- The Google Colaboratory notebook version can be found at [`uk_economic_strategy_text_mining_analysis.ipynb`](/uk_economic_strategy_text_mining_analysis.ipynb)
