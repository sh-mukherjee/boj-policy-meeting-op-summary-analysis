# Sentiment Analysis of Eight Bank of Japan Opinion Summary Reports from Oct 2024 to Sep 2025
Natural Language Processing -- Lexicon-based sentiment analysis of the BoJ Monetary Policy Meeting Opinion Summary reports.

### The Bank of Japan is the central bank of Japan.
"The Bank decides the text of the Outlook for Economic Activity and Prices (Outlook Report) at the Monetary Policy Meetings (MPMs) and releases it quarterly (usually in January, April, July, and October). The Outlook Report presents the Bank's outlook for developments in economic activity and prices, assesses upside and downside risks, and outlines its views on the future course of monetary policy."
The Bank of Japan also publishes a ['Summary of Opinions at the Monetary Policy Meeting'](https://www.boj.or.jp/en/mopo/mpmsche_minu/opinion_all/index.htm), which is a shorter report of 5 to 6 pages and is published around eight times a year.

### The Bank of Japan meeting schedule, reports, and summaries can be found on the Bank of Japan [website](https://www.boj.or.jp/en/mopo/outlook/index.htm/).
We will obtain the text from the pdf files from the links to the last eight summary reports (Oct 2024 to Sep 2025), and use natural language processing to check the sentiment of each report and how it changes over the last couple of years. We will do the analysis using lexicon-based sentiment analysis with specialised lexicons for financial documents.

### Methodology
- Obtain URLs to the online pdf reports from the BoJ website
- Use pdfplumber to read the text in the reports
- Store the dates, URLs and text in a dataframe
- Define the two lexicons used and the dictionary of positive, neutral and negative words
- Count the number of positive and negative words for each report according to each of the two lexicon dictionaries
- Calculate the normalised sentiment scores according to each of the two lexicon dictionaries
- Plot charts showing the results

View my Colab notebook [here](https://colab.research.google.com/github/sh-mukherjee/boj-policy-meeting-op-summary-analysis/blob/main/BoJ_Monetary_Policy_Op_Summary.ipynb).

<img width="1549" height="524" alt="newplot" src="https://github.com/user-attachments/assets/e9e3a939-e6e0-4790-819c-1cf597cc2954" />
