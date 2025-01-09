# Semantic Networks for Hostility Analysis in Tweets

## Overview
This project explores the use of **semantic networks** to analyze hostility in tweets.  
By categorizing words and understanding their relationships, the project aims to uncover patterns in language that correlate with hostile behavior.  
The insights can be applied to social media monitoring, sentiment analysis, and content moderation.

## Objectives
- Create semantic networks from tweets classified by hostility levels: non-hostile, moderately hostile, and highly hostile.
- Use network analysis techniques to identify key features of each hostility level.
- Visualize the results to provide actionable insights.

## Methodology
1. **Data Collection:** Gather tweets and classify them based on hostility levels: non-hostile, moderately hostile, and highly hostile.
2. **Preprocessing:** 
   - Remove noise (e.g., URLs, hashtags, and mentions).
   - Tokenize text and assign words to predefined categories (e.g., curses, emotions, general terms).
3. **Network Construction:** 
   - Build networks for each hostility class.
   - Nodes represent words; edges represent co-occurrence.
4. **Community Detection:** Apply **Louvain** and **Leiden** algorithms to detect word communities.
5. **Visualization:** Use tools like igraph and Matplotlib to visualize the networks and highlight key findings.

## Features
### Word Categories
Words are grouped into predefined categories:
- **Curses:** Profanity and slurs.
- **Emotions:** Positive and negative emotions.
- **General Terms:** Neutral words used frequently.

### Network Analysis Metrics
- **Betweenness Centrality:** Importance of a node in connecting different parts of the network.
- **Closeness Centrality:** Proximity of a node to all others.
- **Modularity:** Strength of division of the network into communities.

### Algorithms
- **Louvain Community Detection:** Optimizes modularity for community identification.
- **Leiden Community Detection:** Improves upon Louvain for better community resolution.

## Results
### Network Comparison
#### Non-Hostile Tweets
- Words are more evenly distributed.
- High modularity indicating clear topic segmentation.

#### Moderately Hostile Tweets
- Dense connections around curses and negative emotions.
- Communities are less distinct compared to non-hostile tweets.

#### Highly Hostile Tweets
- Strong clusters of profanity and negative terms.
- Central nodes include offensive words and emotionally charged terms.

### Metric Insights
#### Betweenness Centrality
- Highly hostile networks show dominant nodes with high centrality (e.g., offensive terms).

#### Closeness Centrality
- Non-hostile networks exhibit balanced closeness, reflecting diverse word usage.


## Code Structure
The repository contains the following:
- **Data Collection:** Scripts for scraping and cleaning tweets.
- **Preprocessing:** Tokenization, word categorization, and stopword removal.
- **Network Analysis:** Functions to compute centrality, modularity, and community detection.
- **Visualization:** Tools for generating visualizations and side-by-side comparisons.

## Evaluation Metrics
- **Modularity Score:** Higher values indicate better community structure.
- **Centrality Metrics:** Identify key nodes and their influence.
- **Graph Density:** Measures the overall connectivity of the network.

## Next Steps
- Adding contextual data (e.g., user metadata) to enhance network richness.
- Comparing results with external hostility datasets.
- Expanding to multilingual analysis.
- Expanding to age groups analysis.


## Data Source
**Kaggle:** [cyberbullying-bystander-dataset](https://www.kaggle.com/datasets/haifasaleh/cyberbullying-bystander-dataset-2023?select=202305_CYBERBYSTANDER+%28CYBY23%29+dataset.xlsx)

## Detailed Presentation
[Cyberbullying Presentation](https://github.com/AlonFeldman15/Semantic-Network-Project/blob/main/Cyberbullying%20Presentation.pdf)

## Contact
**Alon Feldman**  
**Email:** alon.feldman5@gmail.com  
**LinkedIn:** [Alon Feldman](https://www.linkedin.com/in/alon-feldman5)  
**Thanks to:** [Tomer Hod](https://github.com/tomerhod1)  
**Technion - Spring 2024**
