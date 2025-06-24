# NLP-assignment-2

## This is the readme file for question 2.1: Text Vectorization Implementation

Comparison of Word Scores
Manual TF-IDF and scikit-learn's TfidfVectorizer both assign low scores to common words like "the", and higher scores to rare/unique words like "star" or "satellite".

CountVectorizer simply counts word occurrences, so common words like "the" have the same weight as any other word.

Why Do Scores for Common Words Differ?
TF-IDF reduces the importance of words that appear in many documents by assigning them a lower score. This is because such words are less useful for distinguishing between documents.

CountVectorizer treats all words equally, regardless of how common they are.

Therefore, common words like "the" have low TF-IDF scores but high CountVectorizer scores.

Key Takeaways
TF-IDF is better for highlighting words that are important for a specific document but rare across the corpus.

CountVectorizer is simpler but can be dominated by common, uninformative words.

