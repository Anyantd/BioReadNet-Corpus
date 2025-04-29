# BioReadNet-Corpus
BioReadNet: A Transformer-Driven Hybrid Model for Target Audience-Aware Biomedical Text Readability Assessment
📄 Associated Paper

This repository contains the BioReadNet corpus, a bilingual dataset of  20,008 biomedical texts labeled by target audience  (expert adults vs. non-expert adults vs. children). It was built to support audience-aware readability assessment and text simplification of biomedical documents.

## 📦 Dataset Description

The corpus consists of three CSV files:

1. **fr_cochraneWikiviki.csv** - French medical texts
2. **en_CochranePlabaSJK.csv** - English medical texts  
3. **BioReadNet_corpus.csv** - Combined multilingual corpus

### File Structure

All CSV files contain the following columns:
- `texte`: The actual text content
- `type_text`: Original label/type of the text (as classified in source)
- `source`: Source from which the text was extracted
- `label`: Label assigned for our specific classification task
- `lang` (only in BioReadNet_corpus.csv): Language code ('fr' or 'en')

## Data Sources

1. 🇫🇷 **French Data**:
   - Extracted from Cochrane Wikiviki
   - Contains medical texts in French

2. 🇬🇧 **English Data**:
   - Extracted from Cochrane Plaba SJK
   - Contains medical texts in English


🛠 Applications
- Biomedical readability classification
- Text simplification and generation
