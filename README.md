# Are U a Joke Master? Pun Generation via Multi-Stage Curriculum Learning towards a Humor LLM
## Introduction
Although large language models (LLMs) have mastered extensive world knowledge and certain reasoning abilities, their ability to generate humorous sentences remains a challenge. Previous studies have shown that the ability of ChatGPT to generate humorous sentences is limited to generating 25 unique jokes. In this work, we will endow LLMs with the ability to generate humorous puns through the preference learning method. We propose a multi-stage curriculum preference learning framework to optimize pun structure preference and humor preference. Moreover, we improve the Direct Preference Optimization (DPO) algorithm to address the challenges of multi-objective alignment problems. Specifically, in the second stage (humor preference alignment), we adopt our proposed preference triple optimization algorithm, that is, adding samples that meet the structural preference in the first stage (Rumination) to form preference triples with positive samples (Positive) and negative samples (Negative) in the second stage, and improving the traditional DPO loss function to a triple DPO loss function. Experimental results show that the triple loss proposed in this paper can alleviate the problem of catastrophic forgetting existing in multi-objective alignment. Through the training process of the above multi-stage curriculum preference learning, we can obtain an LLM that simultaneously meets structural preference and humor preference, effectively improving the success rate of large models in generating puns.
![model](https://github.com/user-attachments/assets/721804f5-5a3c-4755-b51b-7ee01125d19c)
In addition, to promote further development in this field, we have collected a Chinese pun dataset named ChinesePun, which contains 2.1k puns and corresponding annotations.
![model](https://github.com/user-attachments/assets/51849615-306d-487d-bdc3-8280464a2eb3)
## Results
Comprehensive experimental results on the Chinese (ChinesePun) and English (SemEval) benchmark datasets show that our method (PGCL) is significantly superior to all baseline models.
![main](https://github.com/user-attachments/assets/8e9ff7c8-6e73-4bb1-80bb-c939f624d8e9)
## Citation
If you find this project useful in your research, please consider cite:
```
@inproceedings{chen-etal-2024-u,
    title = "Are {U} a Joke Master? Pun Generation via Multi-Stage Curriculum Learning towards a Humor {LLM}",
    author = "Chen, Yang  and
      Yang, Chong  and
      Hu, Tu  and
      Chen, Xinhao  and
      Lan, Man  and
      Cai, Li  and
      Zhuang, Xinlin  and
      Lin, Xuan  and
      Lu, Xin  and
      Zhou, Aimin",
    editor = "Ku, Lun-Wei  and
      Martins, Andre  and
      Srikumar, Vivek",
    booktitle = "Findings of the Association for Computational Linguistics ACL 2024",
    month = aug,
    year = "2024",
    address = "Bangkok, Thailand and virtual meeting",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.findings-acl.51",
    pages = "878--890",
    abstract = "Although large language models (LLMs) acquire extensive world knowledge and some reasoning abilities, their proficiency in generating humorous sentences remains a challenge. Previous research has demonstrated that the humor generation capabilities of ChatGPT are confined to producing merely 25 unique jokes. In this work, we concentrate on endowing LLMs with the ability of generating puns, a particular category of humor by preference learning method. We propose a multi-stage curriculum preference learning framework to optimize both pun structure preferences and humor preferences. Specifically, we improve the Direct Preference Optimization (DPO) algorithm to address the challenge of multi-objective alignment problem. Besides, to facilitate further advancement in this field, we collect a Chinese Pun (ChinesePun) dataset, containing 2.1k puns and corresponding annotations. Experimental results on both Chinese and English benchmark datasets demonstrate that our method significantly outperforms all the baseline models.",
}
```
