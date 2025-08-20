# Invoice data extraction with Google Gemini (Generative AI)

Ask queries directly to your invoices with Google's Gemini or get the data in JSON

## 📓 How It Works
1. **Authentication**  
   - API key stored securely in Colab Secrets (`GOOGLE_API_KEY`).  
   - Loaded into the notebook and passed to the Gemini client.

2. **Upload Invoice File**  
   - Supported formats: `jpeg`, `png`, `pdf`.  
   - File is uploaded once and reused for multiple queries.

3. **Ask Questions**  
   - Use the helper `ask(question)` function to query invoice details.  
   - The Gemini model processes the document and returns concise answers.

4. **Optional: Structured Output**  
   - Define a schema with **Pydantic** (`Invoice`, `LineItem` models).  
   - Enforce JSON output for clean data ingestion into BI tools or data warehouses.
Use Cases
	•	Automating invoice digitization and data entry.
	•	Extracting financial details for analytics and reporting.
	•	Building chatbot-style interfaces for document understanding.
	•	Feeding structured invoice data into ETL pipelines, BigQuery, or Tableau/Power BI dashboards.