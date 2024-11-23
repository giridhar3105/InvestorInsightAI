# InvestorInsightAI

InvestorInsightAI is an intelligent tool designed to process financial transcripts and extract key investor-relevant insights. The tool leverages advanced NLP techniques, including zero-shot classification and text summarization, to categorize and condense information from company documents.

## Features
- **PDF Text Extraction**: Reads text from company transcripts using `pdfminer.six`.
- **Dynamic Topic Classification**: Categorizes sentences into predefined topics like growth prospects, business changes, and earnings impact using a Hugging Face zero-shot classification model.
- **Summarization**: Summarizes key information for each topic using the BART summarization model.
- **Organized Output**: Presents insights in a JSON format for easy analysis and reporting.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/giridhar3105/InvestorInsightAI.git
   cd InvestorInsightAI
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Upload your PDF transcript.
2. Run the notebook or script to process the document.
3. View categorized and summarized insights in the output JSON.

## Algorithm Workflow
1. **Upload PDF**: Upload a company transcript in PDF format.
2. **Extract Text**: Extract content using `pdfminer.six`.
3. **Classify Sentences**: Use zero-shot classification to categorize content dynamically.
4. **Summarize Insights**: Summarize each category using the BART model.
5. **Save Results**: Output the summarized insights to a JSON file.

## Technologies Used
- `pdfminer.six` for PDF text extraction.
- Hugging Face Transformers for zero-shot classification and summarization.
- `spaCy` for natural language processing.

## Example Output
```json
{
  "growth prospects": "The company aims to expand its market share in Asia.",
  "business changes": "Introduced a new product line targeting younger demographics.",
  "earnings impact": "Projected revenue increase of 15% due to recent acquisitions."
}
```

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for discussion.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
