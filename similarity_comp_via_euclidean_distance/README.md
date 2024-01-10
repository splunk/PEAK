# Chrome Extension Similarity Explorer
**Model-Assisted Threat Hunting** for ***masquerading Chrome Extensions*** </br>

<img src="img/masque.png" width='200' align='right'></img>

This notebook uses quantitative metrics to hunt for similarity that could suggest masquerading, via:
   - **Levenshtein similarity** between **Extension Names**,
   - **Color Moment similarity** between **Extension Icons**,
   - **Cosine Similarity** between **Extension descriptions**,
   - **Unsupervised Learning** to cluster and visualize extension in **3-D Scatterplot**,
   - **Euclidean Distance** as a **composite similarity score**.
   
This threat hunting workflow is described in greater detail on the <a href="https://www.splunk.com/en_us/blog/tag/surge.html">Splunk SURGe</a> Security Research blog.
