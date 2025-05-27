# Indian Music Recommendation System 🇮🇳🎶

A content-based music recommendation system tailored for Indian songs, utilizing Natural Language Processing (NLP) and cosine similarity to suggest similar tracks based on lyrics and metadata.

---

## 📌 Overview

This project focuses on recommending Indian songs by analyzing their lyrics and associated metadata. It employs:

- **TF-IDF Vectorization** for textual feature extraction
- **Cosine Similarity** to measure song similarity
- **Streamlit** for an interactive web interface

---

## 📁 Dataset

The dataset `music_indian.csv` includes metadata and lyrics for Indian songs. Key columns:

- `song`: Title of the song
- `singers`: Artists involved
- `lyricist`: Lyric writer
- `composer`: Music composer
- `lyrics`: Full lyrics of the song
- `tags`: Genre, mood, or other descriptors

---

## 🚀 Features

- Recommends similar songs based on lyrical and metadata analysis
- Clean and interactive UI using Streamlit
- Unicode lyrics support for Hindi and other Indian languages
- Lyrics and metadata preprocessing for improved accuracy

---

## 🧠 How It Works

1. **Preprocessing**  
   Combines `singers`, `composer`, `lyricist`, `lyrics`, and `tags` into a single column. Stopwords and punctuation are removed.

2. **Vectorization**  
   Applies `TfidfVectorizer` to the combined text column to convert it into numeric form.

3. **Similarity Computation**  
   Calculates cosine similarity across all song pairs.

4. **Recommendation Engine**  
   Given a song name, the system recommends the top N most similar songs.

---

## 🖥️ Usage

### 1. Clone the Repository

```bash
git clone https://github.com/vira250/Indian-Music-Recommendation.git
cd Indian-Music-Recommendation

