# 🍽️ Culinary Compass: AI Restaurant Review Analyzer

> Transform restaurant reviews into actionable insights using AI

## 📋 Overview

This project uses AI to analyze restaurant reviews and provide structured insights. Instead of reading through hundreds of reviews manually, get instant sentiment analysis, structured summaries, and answers to specific questions.

## ✨ Features

- **Sentiment Analysis** - Understand customer emotions across multiple reviews
- **Smart Summaries** - Get pros, cons, and recommendation scores in JSON format
- **Q&A System** - Ask specific questions about restaurants and get fact-based answers
- **Live Data** - Fetches real-time reviews from Google Maps

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- OpenAI API Key
- Google Maps API Key

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-restaurant-reviewer.git
cd ai-restaurant-reviewer

# Install dependencies
pip install -r requirements.txt

# Run the notebook
Culinary Compass.ipynb
```

### Usage

```python
# Initialize the AI reviewer
reviewer = SimplifiedRestaurantReviewer(openai_api_key)

# Analyze reviews
search_query = "best pizza in Kuala Lumpur"
reviews = get_Maps_reviews(maps_api_key, search_query)
summary = reviewer.summarize_reviews(reviews)

print(f"Recommendation Score: {summary['Recommendation Score']}/10")
```

## 📊 Sample Output

```json
{
  "PROS": ["Great authentic taste", "Quick service", "Good value"],
  "CONS": ["Limited parking", "Can get crowded"],
  "Overall Summary": "Popular local spot with excellent food",
  "Recommendation Score": 8
}
```

## 🛠️ Tech Stack

- **LangChain** - AI framework
- **OpenAI GPT-3.5** - Language model
- **FAISS** - Vector search
- **Google Maps API** - Review data



## 👨‍💻 Author

**Puteri Irene Alia binti Abdul Hadi**
- Email: puteriirene@gmail.com
- LinkedIn:[ [[Your Profile]](https://www.linkedin.com/in/puteri-irene-alia-abdul-hadi-586a67a7/)]

---
⭐ Star this repo if you found it helpful!
