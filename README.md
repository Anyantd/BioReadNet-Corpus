# BioReadNet-Corpus
BioReadNet: A Transformer-Driven Hybrid Model for Target Audience-Aware Biomedical Text Readability Assessment
📄 Associated Paper

This repository contains the BioReadNet corpus, a bilingual dataset of  20,008 biomedical texts labeled by target audience  (expert adults vs. non-expert adults vs. children). It was built to support audience-aware readability assessment.

## 📦 Dataset Description

The corpus consists of three CSV files:

1. **fr_cochraneWikiviki.csv** - French medical texts -> raw_data.zip
2. **en_CochranePlabaSJK.csv** - English medical texts  -> raw_data.zip
3. **BioReadNet_corpus.csv** - Combined multilingual corpus -> BioReadNet_corpus.zip

### File Structure

All CSV files contain the following columns:
- `texte`: The actual text content
- `type_text`: Original label/type of the text (as classified in source)
- `source`: Source from which the text was extracted
- `label`: Label assigned for our specific classification task
- `lang` (only in BioReadNet_corpus.csv): Language code ('fr' or 'en')

## Data Sources

1. 🇫🇷 **French Data**:
   - Extracted from Cochrane Wikiviki http://natalia.grabar.free.fr/CLEAR/clear-res.php 
   - Contains medical texts in French 

2. 🇬🇧 **English Data**:
   - Extracted from Cochrane Plaba SJK
      - Cochrane https://github.com/qiuweipku/Plain_language_summarization/tree/main/CDSR_data
      - Plaba https://bionlp.nlm.nih.gov/plaba2023/#data
      - SJK https://github.com/loukritia19/science-journal-for-kids-data
   - Contains medical texts in English

Note: You can access Cochrane Reviews for non-commercial text and data mining by accepting Wiley's click-through Text and Data Mining license. Once accepted, you'll receive an API token. Learn more here:
   -Wiley TDM License: https://onlinelibrary.wiley.com/library-info/resources/text-and-datamining
   -Cochrane Access Help: https://www.cochranelibrary.com/help/access

🛠 Applications
- Biomedical readability classification
- Text simplification and generation
- Information retreival 
