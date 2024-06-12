# AMAZON's Product reviews Sentiment: A Natural Language Processing Approach (NLP)

## Description
The project is designed to analyze and classify the sentiment of customer reviews on Amazon products. By leveraging natural language processing (NLP) techniques and sentiment analysis algorithms, the model can determine whether a review expresses a positive, negative, or neutral sentiment. This model provides valuable insights into customer opinions, helping businesses understand consumer satisfaction and areas for improvement.

## Required Libraries
- `pandas` 
- `spacy`
- `datetime`
- `matplotlib`
- `seaborn`
- `spacytextblob.spacytextblob`
- `textblob`

## Dataset
The dataset used in the Amazon Product Reviews Sentiment Model contains 34,660 consumer reviews for 48 Amazon products across 41 categories. Although it does not include explicit sentiment labels, it provides comprehensive information about each review and the products being reviewed. The dataset includes the following columns:

- `id`: A unique identifier for each review entry.
- `name`: The name of the product being reviewed.
- `brand`: The brand of the product.
- `categories`: The categories to which the product belongs.
- `keys`: Keywords associated with the product.
- `manufacturer`: The manufacturer of the product.
- `reviews.date`: The date when the review was written.
- `reviews.dateAdded`: The date when the review was added to the dataset.
- `reviews.dateSeen`: The date when the review was last seen.
- `reviews.didPurchase`: Indicates whether the reviewer purchased the product.
- `reviews.doRecommend`: Indicates whether the reviewer recommends the product.
- `reviews.id`: A unique identifier for the review.
- `reviews.numHelpful`: The number of users who found the review helpful.
- `reviews.rating`: The numerical rating given by the reviewer (e.g., 1 to 5 stars).
- `reviews.sourceURLs`: The URLs of the sources where the review was found.
- `reviews.text`: The text content of the review.
- `reviews.title`: The title of the review.
- `reviews.userCity`: The city of the reviewer.
- `reviews.userProvince`: The province of the reviewer.

## Key Steps

### 1. Data Preprocessing:

- **Convert to String:** Ensure all input text data is in string format to maintain consistency and compatibility with text processing libraries.
- **Lowercase Conversion:** Convert all text to lowercase to ensure uniformity and prevent case-sensitivity issues during analysis.
- **Lemmatization:** Reduce words to their base or root form (e.g., "running" becomes "run") to normalize the text data.
- **Whitespace Stripping:** Remove any leading or trailing whitespace from the text to clean the data.
- **Tokenization:** Break down the text into individual tokens or words, which can be converted into numerical vectors for model input.
- **Stopwords and Punctuation Removal:** Eliminate common stopwords (e.g., "and", "the") and punctuation marks to focus on the meaningful words in the text.

### 2. Sentiment Prediction Using TextBlob:

- **Text Conversion:** Convert the input text to a string format to ensure compatibility with the TextBlob library.
- **TextBlob Object Creation:** Create a TextBlob object from the input text, enabling access to TextBlob's sentiment analysis tools.
- **Polarity Calculation:**
- **Polarity:** Calculate the polarity score of the text, which ranges from -1.0 to 1.0.
- **Positive Polarity:** Indicates a positive sentiment.
- **Negative Polarity:** Indicates a negative sentiment.
- **Polarity of Zero:** Indicates a neutral sentiment.
- **Sentiment Classification:**
Based on the polarity score, classify the sentiment of the text as 'Positive', 'Negative', or 'Neutral'.
Return the sentiment classification as a string.