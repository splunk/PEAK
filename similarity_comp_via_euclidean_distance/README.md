# Chrome Extension Similarity Explorer
**Model-Assisted Threat Hunting** for ***masquerading Chrome Extensions*** </br>
<a href="https://www.splunk.com/en_us/blog/author/rfetterman.html">Dr. Ryan Fetterman</a>

<img src="img/masque.png" width='200' align='right'></img>

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1-_ZupjocfeK-C1lXmVCWnF3rZh4FBr_M?usp=sharing)

This notebook uses quantitative metrics to hunt for similarity that could suggest masquerading, via:
   - **Levenshtein similarity** between **Extension Names**,
   - **Color Moment similarity** between **Extension Icons**,
   - **Cosine Similarity** between **Extension descriptions**,
   - **Unsupervised Learning** to cluster and visualize extension in **3-D Scatterplot**,
   - **Euclidean Distance** as a **composite similarity score**.
   
This threat hunting workflow is described in greater detail on the <a href="https://www.splunk.com/en_us/blog/tag/surge.html">Splunk SURGe</a> Security Research blog, and is intended to be used to explore the Chrome Extension Web Store data, or re-purposed as a means to assess similarity between data points in 3-dimensional space.

This work was presented at the Infosec Jupyterthon 2024. The presentation is hosted <a href="https://github.com/fetterm4n/infosec-jupyterthon">here</a>.
