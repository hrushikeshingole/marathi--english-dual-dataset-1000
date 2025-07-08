
# Mental Health Q&A Dataset with Marathi Translations

## 🧠 Overview
This dataset contains **1,000 question-and-answer pairs** related to mental health, categorized into topics such as **Depression**, **Addiction**, **Anxity** , **PTSD** and **Stress**. Each entry includes the original **English text and its Marathi translation**, supporting AI-driven mental health applications for **Marathi-speaking communities**.

---

## 📁 Dataset Description

**File Name**: `marathi- english dual dataset 1000.csv`  
**Format**: CSV (UTF-8 encoded)  
**Size**: 1000 rows  

### Columns

| Column Name         | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `questionText`      | English question describing a mental health concern                         |
| `answerText`        | English response from a mental health expert                                |
| `category`          | Mental health category (e.g., Depression, Addiction, Stress)                |
| `marathi_question`  | Marathi translation of the question                                         |
| `marathi_answer`    | Marathi translation of the answer                                           |

---

## 🌐 Language & Encoding
- **Languages**: English and Marathi  
- **Encoding**: UTF-8 (supports Devanagari script)  
- **Category Distribution (approx.)**:  
  - Depression: 40%  
  - Addiction:  20%  
  - Stress:     10%
  - Anxity:     30%
  - PTSD:       10%

---

## 🔍 Features

- **Bilingual Content** for multilingual mental health research and tools  
- **Categorized Data** for topic-specific NLP/ML training  
- **Real-world Mental Health Context** (e.g., trauma, recovery, emotional distress)  
- **Structured Format** (CSV) compatible with NLP pipelines and knowledge graphs  
- **Sensitive Data Handling**: Anonymized, with ethical considerations

---

##  Potential Use Cases

- **AI Chatbots**: Train conversational agents (e.g., BERT, mBART)  
-  **Sentiment Analysis** on user emotional tone  
-  **Knowledge Graph Construction**: Build relationships like `Symptom → Disorder → Treatment`  
-  **Cross-Lingual NLP** for machine translation and zero-shot learning  
-  **Mental Health Education** and content localization  
-  **Multilingual Dialogue Corpora** for research and benchmarking

---

##  Data Collection

- **Source**: English Q&A data collected from [insert actual source, e.g., public forums, expert input]  
- **Translation**: Marathi generated via [insert actual method, e.g., Google Translate + Human verification]  
- **Categorization**: Manual or rule-based assignment to 3 primary categories

---

##  Preprocessing Instructions

```python
import pandas as pd
df = pd.read_csv("marathi- english dual dataset 1000.csv", encoding='utf-8')

# Check for missing values
print(df.isnull().sum())

# Remove duplicates
df = df.drop_duplicates()

# Normalize categories
df['category'] = df['category'].str.title()

# Clean whitespace
df['questionText'] = df['questionText'].str.strip()
df['marathi_question'] = df['marathi_question'].str.strip()
```

Optional:
```python
from nltk.tokenize import word_tokenize
df['questionText_tokens'] = df['questionText'].apply(word_tokenize)
```

---

## ⚠️ Ethical Considerations

- **Sensitive Content**: Topics like trauma, abuse, addiction – use with care  
- **No Personal Identifiers (PII)**  
- **Culturally Validated** Marathi content recommended before deployment  
- **Use Responsibly**: For positive mental health impact only  
- **Legal**: Ensure DPDP Act (India) compliance where applicable

---

## 📎 Example Row (CSV)

```
questionText,answerText,category,marathi_question,marathi_answer
"I have so many issues to address...","It is very common for people to have multiple issues...","Depression","माझ्याकडे लैंगिक अत्याचाराचा इतिहास आहे...","लोकांनी असा प्रश्न विचारला आहे की त्यांना समुपदेशनात..."
```

---

## 📜 License

This dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)**.  
You may share, adapt, and use this dataset with **appropriate attribution**.

---

## 📚 Citation

```
[Your Name or Organization]. (2025). Mental Health Q&A Dataset with Marathi Translations. [Repository Name].
```

---

## 📫 Contact

For queries, improvements, or collaboration:  
📧 Email: [Hrushikeshingole75@gmail.com]  
💬 GitHub: [your_repo_link]

---


