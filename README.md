
# grcAssist

This program is designed to pull relevant current news articles for keywords defined in a `keywords.csv` file. GRC (Governance, Risk Management, and Compliance) professionals can use this to build a bank of quick-to-access relevant cyber news stories or for a Just-in-Time news story to educate end users.

## Getting Started

### Prerequisites

- Python 3.x
- `requests` library (install via `pip install requests`)
- `openpyxl` library (install via `pip install openpyxl`)
- An API key from [NewsData.io](https://newsdata.io/)

### Setting Up Your API Key

To access the news articles, you need to obtain an API key from NewsData.io. Follow these steps:

1. Visit [NewsData.io](https://newsdata.io/) and sign up for an account.
2. Once you have registered, log in to your account and navigate to the "API Keys" section.
3. Generate a new API key.
4. Copy the generated API key.

Next, you need to paste this API key into the Python code:

1. Open the Python script file that contains the line `api_key = "YOUR_API_KEY_HERE"`.
2. Replace `"YOUR_API_KEY_HERE"` with your actual API key. The line should look like this:

   ```python
   api_key = "YOUR_ACTUAL_API_KEY"
   ```

3. Save the file.

### Updating the `keywords.csv` File

The `keywords.csv` file is where you define the keywords for which you want to fetch news articles. Each line in the file should contain one keyword or keyword combination. 

**Important:** Use `%20` to represent spaces between words in a keyword combination. Here are some examples of how to format your keywords:

```plaintext
cybersecurity%20healthcare
cybersecurity%20regulations
data%20privacy%20laws
cloud%20security
```

Make sure to save the `keywords.csv` file after adding or updating your keywords!

### Running the Program

Once you have set up your API key and updated the `keywords.csv` file with your desired keywords:

1. Run the Python script using the following command:
   ```bash
   python grcAssist.py
   ```
2. The program will pull relevant news articles based on the keywords provided and display them in the output or save them to a file (as specified in the code).

---
This python application is originally from https://github.com/gerryguy311/grcAssist