# PEAK Model-Assisted Threat Hunting for Dictionary DGA

This notebook was created in conjunction with the Splunk SURGe <a href="https://www.splunk.com/en_us/blog/security/threat-hunting-for-dictionary-dga-with-peak.html" target="_blank">"Threat Hunting for Dictionary-DGA"</a> blog post, to demonstrate development of Model-Assisted Threat Hunting approach for detecting Dictionary-based Domain Generation Algorithms, as part of the PEAK Threat Hunting Framework. Two notebooks are provided: `m-ath-dictionary-dga-pretrain_dsdl.ipynb` for use in the the Splunk Deep Science and Deep Learning (DSDL) Toolkit, or `m-ath-dictionary-dga-pretrain_local.ipynb`, for stand-alone use.

<img src="https://www.splunk.com/content/dam/splunk-blogs/images/en_us/2022/05/fetterman-math-conclusions.png" alt="PEAK Threat Hunting, by SURGe" style="width: 30%;">

### Pre-requisite

- This notebook was built using the Splunk Deep Science and Deep Learning (DSDL) Toolkit, however it will work in any Jupyter / JupyterLab environment with the correct packages and dependencies.
- The `requirements.txt` file is only necessary if running outside of a DSDL environment.

### Setup

From the DSDL JupyterLab, use the Upload option, or drag-and-drop the downloaded files from this repository into the correct paths following these steps:

- Upload `m-ath-dictionary-dga-pretrain.ipynb` to the `notebooks` directory
- Upload `dict_dga.json` to the `/srv/notebooks/data` folder
- Upload `m-ath_dict_dga_model.zip`, `m-ath_pretrain_tokenizer.pkl`, and `m-ath_pretrain_word_list.pkl` to the `/srv/app/model/data folder`
    - Open a new tab in JupyterLab to the Terminal
    - Extract the model files by using the command `unzip m-ath_dict_dga_model.zip`
- Follow instructions in notebook (Stage 1) to stage the domain data you want to hunt into the notebook environment.
    - NOTE: Your staging command must use algo=dict_dga for the notebook to work without modification. e.g., `| fit MLTKContainer mode=stage algo=dict_dga domain into app:dict_dga`
- Run the notebook by executing each cell (Shift + Enter), or the JupyterLab run all cells option '⏭'

#### For Local Use
- Clone the repository using `git clone git@github.com:splunk/PEAK.git`
- Upzip `m-ath_dict_dga_model.zip`
- Run `m-ath-dictionary-dga-pretrain-local.ipynb`


