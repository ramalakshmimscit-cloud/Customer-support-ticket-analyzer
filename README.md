# Customer Support Ticket Analyzer 🎫

A robust Python-based tool for managing, cleaning, and analyzing customer support tickets. This project automates the workflow from raw data entry to sentiment-based insights.

## 🚀 Features
- **Ticket Management**: Pre-loaded with 10 tickets; supports dynamic user additions with auto-incrementing IDs.
- **Data Validation**: Strict enforcement of priority levels (High, Medium, Low).
- **Text Normalization**: Custom cleaning function that:
  - Removes punctuation.
  - Converts text to lowercase.
  - Normalizes slang (e.g., "ok" → "okay").
- **Analytical Insights**: 
  - Keyword frequency tracking (Good, Poor, Slow, etc.).
  - Priority distribution reporting.
  - Complexity analysis via word counts.

## 🛠️ Installation
1. Clone the repository:
   ```bash
   git clone https://github.com
   ```
2. Open the file in **Google Colab** or any Python 3.x environment.

## 💻 Code Usage
The core logic utilizes a dictionary of lists for data storage and a custom cleaning function:

```python
def clean_text(text):
    text = text.lower()
    for char in ".,!?-":
        text = text.replace(char, "")
    return " ".join(text.split()).strip()
```

## 📊 Sample Output
Upon running the script, you will receive:
- A count of tickets categorized by priority.
- Sentiment analysis based on keyword occurrences.
- Identification of the most complex (longest) ticket.

## 📂 Project Deliverables
- `Customer_Support_Analyzer.ipynb`: Main Python source code.
- `Project_Summary.pdf`: One-page executive summary of findings.

