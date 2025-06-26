# Sentiment Analysis and Emotional Comparison of U.S. Presidential Speeches

This project analyzes the sentiment and emotional intensity in speeches by **Abraham Lincoln** and **Benjamin Harrison**, using modern NLP tools. The goal is to explore how their speech tones vary in terms of positivity and emotional depth, providing insights into political communication styles.

---

## 📚 Data Sources

1. **Abraham Lincoln**  
   - [Project Gutenberg: Speeches, 1832–1865](https://www.gutenberg.org/cache/epub/14721/pg14721-images.html)

2. **Benjamin Harrison**  
   - [Project Gutenberg: Presidential Speeches](https://www.gutenberg.org/cache/epub/44682/pg44682-images.html)

These texts were scraped using `requests` and `BeautifulSoup`, filtered to retain only meaningful paragraph content.

---

## 🛠️ Technologies Used

- **Python 3.10+**
- `Flair` – Sentiment analysis using `en-sentiment` model
- `Pandas`, `Matplotlib`, `Seaborn` – Data manipulation and visualization
- `WordCloud` – For visualizing emotionally intense words
- `BeautifulSoup`, `requests` – Web scraping

---

## 🧪 Methodology

### Q1. Which president used more **positive vs. negative** language?
- Counted sentiment predictions for each sentence.
- Visualized with a bar plot grouped by sentiment and president.

### Q2. Who used more **emotionally intense** language?
- Averaged the sentiment confidence scores for each president.
- Compared using grouped bar plots.

### Q3. Is there a difference in emotional intensity between **positive and negative** sentiments?
- Boxplot used to visualize intensity variation split by sentiment and source.

### Bonus: Word clouds
- Displayed the most emotionally intense words (based on top 100 high-confidence sentences) for each president.

---

## 📊 Visual Output

- **Sentiment Polarity Distribution**  
  Shows how many positive vs. negative sentences were found for each president.

- **Emotional Intensity Boxplot**  
  Compares how intense (confident) each sentiment was across presidents.

- **Average Sentiment Confidence Bar Plot**  
  Shows which president consistently used more intense language.

- **Word Clouds**  
  Highlights the most emotionally charged words from top scoring sentences.

---

## 📁 Output Files

| File Name                                | Description                                                  |
|------------------------------------------|--------------------------------------------------------------|
| `sentence_level_sentiments.csv`          | All sentences with predicted sentiment and confidence score  |
| `sentiment_summary_by_president.csv`     | Summary stats: sentiment counts and averages by president    |
| `lincoln_harrison_raw_text.txt`          | Full scraped speeches of both presidents                     |
| `Mini Project Report_ArchitDukhande.pdf` | Final write-up and analysis document                         |

---

## 🧾 Instructions to Run

1. Clone this repo or download the files.
2. Install required packages:
   ```bash
   pip install flair pandas matplotlib seaborn wordcloud beautifulsoup4 requests
