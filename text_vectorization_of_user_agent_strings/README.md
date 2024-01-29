# Text Vectorization of User Agent Strings
<img src="https://www.splunk.com/content/dam/splunk-blogs/images/en_uk/2024/1/useragent1.jpg" width='200' align='right'></img>

In this approach, user agent-strings are encoded via a vector database to enable a model-assited threat hunting workflow:

This methodology allows us to:
- (0) parse the user agent string into a set of tokens or string elements
- (1) Hash each token, and convert it to a number
- (2) Produce a pseudo-random number specific to this particular token.
- (3) Create a numerical signature using this list of numbers, a signature that can then be used to compare user agents.

Blog: <a href="https://www.splunk.com/en_us/blog/tips-and-tricks/text-vectorisation-clustering-and-similarity-analysis-with-splunk-exploring-user-agent-strings-at-scale.html">"Text Vectorisation, Clustering and Similarity Analysis With Splunk: Exploring User Agent Strings at Scale"</a> Author: <a href="https://www.splunk.com/en_us/blog/author/jcowling.html"</a>Josh Cowling
Code: [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/splunk/splunk-mltk-container-docker/tree/master/beta_content)



