# HiddenCut

This repo contains codes for the following paper:

Jiaao Chen, Dinghan Shen, Weizhu Chen, Diyi Yang: HiddenCut: Simple Data Augmentation for Natural Language
Understanding with Better Generalization. ACL 2021

If you would like to refer to it, please cite the paper mentioned above.

## Natural Language Undertanding 
### Prerequisite: 
* CUDA, cudnn
* Python 3.7
* PyTorch 1.4.0



### Run HiddenCut
1. Install Huggingface Transformers according to the instructions here: https://github.com/huggingface/transformers.

2. Download the datasets from the GLUE benchmark:
```python
python download_glue_data.py --data_dir glue_data --tasks all
```

3. Fine-tune the RoBERTa model with the *HiddenCut* data augmentation strategies:
```python
>>> chmod +x run_glue_hidden_cutoff.sh
>>> ./run_glue_hidden_cutoff.sh
```



# Acknowledgement

This repository is built upon https://github.com/dinghanshen/Cutoff


