# Gold-Related Stock Market News Extractor
This Jupyter notebook is designed to extract and summarize gold-related stock market news from a PDF file. It uses various libraries and AI models to process the information and generate a concise report.

# Steps
- PDF Parsing: Uses PyPDFLoader to extract text from a PDF file.
- Keyword Filtering: Filters pages based on specified keywords related to gold stocks and market indices.
- Date Extraction: Utilizes GPT-4 to extract and standardize dates from the text.
- News Extraction: Employs GPT-4 to extract relevant news items from the filtered pages.
- News Summarization: Summarizes the extracted news, grouping it by date.
- PDF Report Generation: Creates a formatted PDF report containing the summarized news.