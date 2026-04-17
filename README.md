# Tolkien NLP Analysis: The Fellowship of the Ring Complexity

This project provides a linguistic analysis of J.R.R. Tolkien's *The Fellowship of the Ring*. Using Natural Language Processing (NLP), I analyzed the text to determine its real reading difficulty based on the CEFR (Common European Framework of Reference for Languages) levels.

## Project Goal
The main objective was to answer a common question: **"How difficult is it to read Tolkien in the original?"**. 
I separated standard English vocabulary from Tolkien-specific "Lore" (names, places, invented terms) to see the actual cognitive load on a learner.

## Tech Stack
- **Language:** Python 3.x+
- **NLP Library:** `spaCy` (Model: `en_core_web_lg`)
- **Data Analysis:** `Pandas`, `NumPy`
- **Regex:** For advanced text cleaning and phrasal verb detection.

## Methodology
* *Lemmatization:** All words were reduced to their dictionary form (e.g., *ran, running, runs* -> *run*).
* *Vocabulary Mapping:** Used a custom dictionary of 10,000+ words categorized by CEFR levels (A1 to C2).
* *Lore Detection:** Proper nouns and unique middle-earth terms were isolated to avoid skewing the language difficulty results.
* *Text Density vs. Unique Vocabulary:** - Analyzed **Unique Words** to see the "vocabulary barrier."
* *Analyzed Total Occurrences** to see the "reading fluency" (how much of the total text is actually understood).

## Key Insights
- **Reading Comfort:** Approximately **85% of the total text** consists of words from A1 to B2 levels.
- **Vocabulary Barrier:** Over **50% of unique words** used in the book are either high-level (C1/C2) or part of the Tolkien Lore.
- **Conclusion:** The analysis reveals that while the Vocabulary Barrier is high (50% unique rare words), the Narrative Foundation is accessible.
85% Comprehension: A reader with a B1/B2 level understands the vast majority of the total word count.
Atmospheric Difficulty: The perceived complexity comes from "low-frequency" words (lore and rare adjectives) that set the mood but don't hide the plot.
Final Verdict: The book is highly readable for intermediate learners who familiarize themselves with core character names beforehand..

## How to Run
1. Clone the repository.
2. Install dependencies: `pip install pandas spacy`.
3. Download the spaCy model: `python -m spacy download en_core_web_lg`.
4. Place your text file (e.g., `fellowship_of_the_ring.txt`) in the root directory.
5. Run the Jupyter Notebook `Untitled-1.ipynb`.

*Note: The full text of the book is not included due to copyright restrictions.*
