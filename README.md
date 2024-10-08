# Gold-Related Stock Market News Extractor
This Jupyter notebook is designed to extract and summarize gold-related stock market news from a long PDF file. Last tested with 250+ pages.

# What problem does it solve?

Analyzing and searching through long PDF files is a pain. This tool does this for you. Of course it can altered easily to search for other topics.

# Technologies used
- langchain
- OpenAI API
- PyPDFLoader

# Steps
- PDF Parsing: Uses PyPDFLoader to extract text from a PDF file.
- Keyword Filtering: Filters pages based on specified keywords related to gold stocks and market indices.
- Date Extraction: Utilizes GPT-4 to extract and standardize dates from the text.
- News Extraction: Employs GPT-4 to extract relevant news items from the filtered pages.
- News Summarization: Summarizes the extracted news, grouping it by date.
- PDF Report Generation: Creates a formatted PDF report containing the summarized news.

# How can be improved?
- If needed, the keyword filter can be made more sophisticated or completely replaced with a semantic search/hybrid approach.
- Better pdf formatting.

# What issues did I encounter?
- The date extraction was not 100% accurate because it relied on the LLM to extract the date in a certain format. To fix this I intruduced regex search for the date at the beginning of each page.
- Hitting the output limit for the gpt-4o model. I had to split the news extraction into smaller chunks and analyze them by date instead of all at once which worked only for smaller files.
