
# Bank of England Financial Risk NLP Pipeline

This project was developed as part of a team assignment in collaboration with the Bank of England. We were tasked with identifying emerging risks in global systematically important banks (G-SIBs) using quarterly earnings call transcripts.

The objective was to extract insights from unstructured financial conversations by detecting sentiment shifts, evasive responses, and topics of concern using modern NLP tools and large language models.

## Project Highlights

• End-to-end NLP pipeline for financial Q&A analysis
• Phi-3.5-based summarisation and topic classification
• Evasion detection to flag unanswered or deflected questions
• BERTopic to identify thematic clusters in evasive and negative responses
• Ground truth data creation for evaluation and model calibration
• Synthetic Q&A generation to test model consistency and avoid data leakage
• Data visualisations including wordclouds, heatmaps, bar charts, and Venn diagrams
• Insights contextualised with financial metrics such as CET1, NII, and EPS

## My Contributions

I worked across the full project lifecycle:

• Defined the problem and project structure with a focus on regulatory risk
• Preprocessed transcripts, paired Q&A, and cleaned text
• Co-developed the Phi-3.5 NLP pipeline:
  - Summarised question-answer pairs using a topic-aware LLM prompt
  - Categorised responses by financial topic such as Strategy, CET1, and Dividends
  - Flagged evasive responses using custom prompt logic
  - Structured outputs using PrettyTable for clarity and readability
• Designed synthetic data to benchmark topic classification and evasion detection
• Built and tested a small ground truth dataset to validate outputs across models
• Interpreted BERTopic outputs and helped integrate results into our final report
• Drafted the executive summary and conclusions, highlighting capital market and reserve concerns across quarters

While the BERTopic clustering and RoBERTa sentiment scoring were led by teammates, I contributed to the interpretation and integration of their results into our reporting.

## Technologies Used

• phi-3.5 for summarisation, classification, and evasion detection
• BERTopic for topic modeling
• PrettyTable, Matplotlib, Seaborn, Venn2, WordCloud
• Pandas, Scikit-learn, spaCy

## Repository Contents

• phi_pipeline/: Co-authored pipeline for summarisation, classification, and evasion detection
• notebook_overview.ipynb: Cleaned high-level walkthrough of the full project
• visuals/: Key outputs including BERTopic and wordcloud plots

## Data Sources

The primary dataset for this project consisted of quarterly earnings call transcripts from global systemically important banks (G-SIBs). These transcripts are publicly available online through company investor relations pages and financial reporting services.

For academic research purposes, a curated subset of these transcripts was compiled and structured into Q&A format. While the original transcripts are public, the annotated and processed dataset we used is not redistributed here. Instead, dummy examples and synthetic Q&A data are provided in the phi_pipeline/ folder to demonstrate structure and functionality.

## Why This Project Matters

This project demonstrates the application of large language models to financial risk monitoring, regulatory insight generation, and the detection of evasive responses from company executives. The methodology is scalable and supports better understanding of emerging risks within financial disclosures.

## Contact

Please get in touch via [LinkedIn](#) or email if you would like to discuss this work or explore collaboration.
