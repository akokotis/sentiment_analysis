# sentiment_analysis
sentiment and part of speech analysis on product reviews

### Goal
- end-to-end process to add sentiment score to user product reviews
- sentiment score can be used when rating is not available
- extract part of speech to understand what words customers are using to describe the products

### Method
1. text cleaning (remove special characters, lowercase, change contractions to full words, replace negated phrases with single words, remove stopwords)
2. annotate reviews with POS model via udpipe package (R)
3. apply sentiment model via udpipe and Bing sentiment - incorporate dependency parsing and polarity shifters
4. validate sentiment scores against existing ratings - precision, recall, Fscore measures
5. export to database for dashboard consumption
