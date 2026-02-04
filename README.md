# Wikipedia Research Assistant (Fraud & Anti-Fraud)

An end-to-end Wikipedia research assistant that:
1) scrapes multiple related Wikipedia pages,
2) extracts structured fields using OpenAI + Pydantic (validated JSON),
3) answers domain questions via tool/function calling (including semantic fuzzy matching).

## Project Files
- Notebook: `Junyi Zhang_Assignment1.ipynb`

## Domain & Articles
Focus: fraud / anti-fraud technologies & practices.

Articles used (7):
- Fraud: https://en.wikipedia.org/wiki/Fraud
- Credit card fraud: https://en.wikipedia.org/wiki/Credit_card_fraud
- Internet fraud: https://en.wikipedia.org/wiki/Internet_fraud
- Phishing: https://en.wikipedia.org/wiki/Phishing
- Multi-factor authentication: https://en.wikipedia.org/wiki/Multi-factor_authentication
- Data analysis for fraud detection: https://en.wikipedia.org/wiki/Data_analysis_for_fraud_detection
- Regulatory technology: https://en.wikipedia.org/wiki/Regulatory_technology

## Structured Schema (Pydantic)
Fields extracted (8):
- tech_name
- summary
- evolution_timeline (year, event)
- key_innovations
- contributors
- applications
- challenges
- mitigations

## Key Features
- Scraping + cleaning pipeline (remove references/footnotes noise, keep main body)
- Robust API calls (rate limit handling + retries/backoff)
- Tool-based Q&A via function calling
- Semantic fuzzy matching (embeddings + cosine similarity, tunable threshold)

## Demo (What to Look For)
Open `Junyi Zhang_Assignment1.ipynb` and check these sections:
- **Scraping demo**: crawl 7 Wikipedia articles and show cleaned text preview
- **Structured extraction demo**: JSON outputs validated by Pydantic (8-field schema)
- **Function calling demo**: compare technologies and return overlaps/differences
  - includes fuzzy matching using embeddings + cosine similarity

## Reproducibility Notes
- API credentials are intentionally omitted for security and course policy compliance.
- The notebook contains saved outputs and examples demonstrating scraping, structured extraction, and function calling.
