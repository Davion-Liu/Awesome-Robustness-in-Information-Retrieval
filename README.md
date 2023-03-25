<p align="center">
  <br>
  <img width="200" src="./imgs/logo.svg" alt="logo of awesome repository">
  <br>
  <br>
</p>

# Awesome Adversarial Attacks and Defenses for Information Retrieval

> A curated list of awesome papers related to adversarial attacks and defenses for information retrieval(IR). If I missed any papers, feel free to open a PR to include them! And any feedback and contributions are welcome! 

We thank all the great contributors very much.

## Contents

- [Adversarial Attack](#adversarial-attack)
	* [Classical Black-hat SEO (Spamming)](#classical-black-hat-seo-(spamming))  
	* [White-hat SEO](#white-hat-seo)        
	* [Neural Methods for IR Attack](#neural-methods-for-ir-attack) 
- [Defense](#defense)
	* [Adversarial Training](#adversarial-training)  
	* [Certified Robustness](#certified-robustness) 
	* [Out-of-distribution in Dense Retrieval](#out-of-distribution-in-dense-retrieval)       
	* [Out-of-distribution in NRM](#out-of-distribution-in-nrm) 
	* [Query Variations](#query-variations) 
- [Benchmark and Evaluation](#benchmark-and-evaluation)
- [Perspective Papers](#perspective-papers)
- [Adversarial Attack and Defense for Image Retrieval](#adversarial-attack-and-defense-for-image-retrieval)
- [Other Resources](#other-resources)






## Adversarial Attack

### Classical Black-hat SEO (Spamming)
- [Web Spam Taxonomy.](http://ilpubs.stanford.edu:8090/771/1/2005-9.pdf) *Zoltan Gyongyi  et.al.* AIRWeb 2005.(**Web Spamming**)
- [International Workshop on Adversarial Information Retrieval on the Web.](http://www.ra.ethz.ch/cdstore/www2008/www2008.org/papers/pdf/p1267-castilloA.pdf)  AIRWeb 2005-2009.
- [Adversarial web search.](https://www.nowpublishers.com/article/DownloadSummary/INR-021) *Castillo, Carlos, and Brian D. Davison* FnTIR 2011.

### White-hat SEO

- [Ranking-Incentivized Quality Preserving Content Modification.](https://arxiv.org/pdf/2005.12989) *Goren Gregory et.al.* SIGIR 2020.

### Neural Methods for IR Attack

- [One word at a time: adversarial attacks on retrieval models.](https://arxiv.org/pdf/2008.02197) *Raval, Nisarg, and Manisha Verma* Arxiv 2020.(**White-box**)
- [Adversarial Semantic Collisions.](https://arxiv.org/pdf/2011.04743) *Congzheng Song et.al.* EMNLP 2020.(**White-box**)
- [Bert rankers are brittle: A study using adversarial document perturbations.](https://arxiv.org/pdf/2206.11724) *Yumeng Wang et.al.* ICTIR 2022.(**White-box**)
- [PRADA: Practical Black-Box Adversarial Attacks against Neural Ranking Models.](https://arxiv.org/pdf/2204.01321) *Chen Wu et.al.* TOIS 2022.(**Black-box**)
- [Order-Disorder: Imitation Adversarial Attacks for Black-box Neural Ranking Models.](https://arxiv.org/pdf/2209.06506.pdf) *Jiawei Liu et.al.* CCS 2022.(**Black-box**)

## Defense

### Adversarial Training

- [IRGAN: A Minimax Game for Unifying Generative and Discriminative Information Retrieval Models](https://arxiv.org/pdf/1705.10513) *Wang, Jun, et al.* SIGIR 2017.(**IRGAN**)
- [Adversarial Sampling and Training for Semi-Supervised Information Retrieval](https://arxiv.org/pdf/1811.04155) *Park, Dae Hoon, Yi Chang* WWW 2019.(**AdvIR**)
- [Adversarial Retriever-Ranker for dense text retrieval](https://arxiv.org/pdf/2110.03611) *Zhang, Hang, et al.* ICLR 2022.(**AR2**)
- [Dealing with textual noise for robust and effective BERT re-ranking](https://www.sciencedirect.com/science/article/pii/S0306457322002369) *Chen, Xuanang, et al.* IPM 2023.
- [A Study on FGSM Adversarial Training for Neural Retrieval](https://arxiv.org/pdf/2301.10576) *Lupart, Simon, Stéphane Clinchant* ECIR 2023.

### Certified Robustness

- [Certified Robustness to Word Substitution Ranking Attack for Neural Ranking Models](https://arxiv.org/pdf/2209.06691.pdf) *Chen Wu et.al.* CIKM 2022

### Out-of-distribution in Dense Retrieval

Looking for [Zero-shot/Few-shot in Dense Retrieval Models](https://github.com/caiyinqiong/Semantic-Retrieval-Models#dense-retrieval-methods) collected by *Yinqiong Cai*.

### Out-of-distribution in NRM

- [Cross Domain Regularization for Neural Ranking Models using Adversarial Learning](https://dl.acm.org/doi/pdf/10.1145/3209978.3210141) *Cohen, Daniel, et al.* SIGIR 2018.
- [Few-Shot Text Ranking with Meta Adapted Synthetic Weak Supervision](https://arxiv.org/pdf/2012.14862) *Si Sun et al.* ACL 2021.(**MetaAdaptRank**)
- [Contrastive Fine-tuning Improves Robustness for Neural Rankers](https://arxiv.org/pdf/2105.12932) *Xiaofei Ma et al.* ACL 2021.
- [Learning List-Level Domain-Invariant Representations for Ranking](https://arxiv.org/pdf/2212.10764) *Ruicheng Xian et al.* Arxiv 2022.(**ListDA**)

### Query Variations


- [Dealing with Typos for BERT-based Passage Retrieval and Ranking](https://arxiv.org/pdf/2108.12139) *Shengyao Zhuang et al.* EMNLP 2021.(**DRTA**)
- [Towards Robust Dense Retrieval via Local Ranking Alignment](https://www.ijcai.org/proceedings/2022/0275.pdf) *Xuanang Chen et al.* IJCAI 2022.(**RoDR**)
- [Evaluating the Robustness of Retrieval Pipelines with Query Variation Generators](https://arxiv.org/pdf/2111.13057) *Penha Gustavo et al.* ECIR 2022.
- [CharacterBERT and Self-Teaching for Improving the Robustness of Dense Retrievers on Queries with Typos](https://arxiv.org/pdf/2204.00716) *Shengyao Zhuang et al.* SIGIR 2022.(**CBST**)
- [Analysing the Robustness of Dual Encoders for Dense Retrieval Against Misspellings](https://arxiv.org/pdf/2205.02303) *Sidiropoulos Georgios et al.* SIGIR 2022.(**DACL**)


## Benchmark and Evaluation

- [Are Neural Ranking Models Robust?](https://arxiv.org/pdf/2108.05018.pdf) *Chen Wu et.al.* TOIS 2022
- [Evaluating Interpolation and Extrapolation Performance of Neural Retrieval Models.](https://dl.acm.org/doi/pdf/10.1145/3511808.3557312) *Jingtao Zhan et.al.* CIKM 2022

## Perspective Papers

- [Competitive Search.](https://dl.acm.org/doi/pdf/10.1145/3477495.3532771) *Oren Kurland et.al.* SIGIR 2022.(**Competitive Search**)
- [A Game Theoretic Analysis of the Adversarial Retrieval Setting.](https://www.jair.org/index.php/jair/article/download/11104/26296) *Basat, Ran Ben et.al.* JAIR 2017.(**PRP is sub-optimal**)

## Adversarial Attack and Defense for Image Retrieval

- [Targeted Mismatch Adversarial Attack: Query with a Flower to Retrieve the Tower](http://openaccess.thecvf.com/content_ICCV_2019/papers/Tolias_Targeted_Mismatch_Adversarial_Attack_Query_With_a_Flower_to_Retrieve_ICCV_2019_paper.pdf) *Giorgos Tolias et al.* ICCV 2019.(**TMA**)
- [Universal Perturbation Attack Against Image Retrieval](https://openaccess.thecvf.com/content_ICCV_2019/papers/Li_Universal_Perturbation_Attack_Against_Image_Retrieval_ICCV_2019_paper.pdf) *Jie Li et al.* ICCV 2019.(**UAP**)
- [Adversarial Ranking Attack and Defense](https://arxiv.org/pdf/2002.11293) *Mo Zhou et al.*ECCV 2020.(**Candidate Attack and Query Attack**)
- [You See What I Want You to See: Exploring Targeted Black-Box Transferability Attack for Hash-based Image Retrieval Systems](https://openaccess.thecvf.com/content/CVPR2021/papers/Xiao_You_See_What_I_Want_You_To_See_Exploring_Targeted_CVPR_2021_paper.pdf) *Yanru Xiao et al.*CVPR 2021.(**Hash-based: Noise-induced Adversarial Generation**)
- [Practical Relative Order Attack in Deep Ranking](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhou_Practical_Relative_Order_Attack_in_Deep_Ranking_ICCV_2021_paper.pdf) *Mo Zhou et al.* ICCV 2021.
- [QAIR: Practical Query-efficient Black-Box Attacks for Image Retrieval](http://openaccess.thecvf.com/content/CVPR2021/papers/Li_QAIR_Practical_Query-Efficient_Black-Box_Attacks_for_Image_Retrieval_CVPR_2021_paper.pdf) *Xiaodan Li et al.* CVPR 2021.(**Query-based Attack against Image Retrieval**)
- [ARRA: Absolute-Relative Ranking Attack against Image Retrieval](https://dl.acm.org/doi/abs/10.1145/3503161.3548138) *Siyuan Li et al.* MM 2022.(**ARRA**)

## Other Resources

- [CREDENCE: Counterfactual Explanations for Document Ranking](https://arxiv.org/pdf/2302.04983) *Rorseth Joel et al.* Arxiv 2023. [Webpage of interactive tool](http://lg-research-1.uwaterloo.ca:8091/credence/builder)







