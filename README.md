<p align="center">
  <br>
  <img width="200" src="./imgs/logo.svg" alt="logo of awesome repository">
  <br>
  <br>
</p>

# Awesome Robustness in Information Retrieval

> A curated list of awesome papers related to robustness, adversarial attacks & defenses, and out-of-distribution data for information retrieval(IR). If I missed any papers, feel free to open a PR to include them! Any feedback and contributions are welcome! 

We thank all the great contributors very much.

## Contents

- [Adversarial Attack](#adversarial-attack)
	* [Classical Black-hat SEO (Spamming)](#classical-black-hat-seo-(spamming))  
	* [White-hat SEO](#white-hat-seo)        
	* [Neural Methods for IR Attack](#neural-methods-for-ir-attack) 
- [Defense](#defense)
	* [Adversarial Training (improving effectiveness)](#adversarial-training)  
	* [Certified Robustness](#certified-robustness)
	* [Detection](#detection)
- [Out-of-distribution](#out-of-distribution)
	* [Data Augmentation](#data-augmentation)
	* [Domain Modeling](#domain-modeling)
	* [Architectural Modifications](#architectural-modifications)
	* [Scaling up the Model Capacity](#scaling-up-the-model-capacity)
	* [Continual Learning for Generative Retrieval](#continual-learning-for-generative-retrieval)
	* [Continual Learning for Dense Retrieval](#continual-learning-for-dense-retrieval)
	* [Query Variations](#query-variations)
	* [Unseen Query Type](#unseen-query-type)
- [Benchmark and Evaluation](#benchmark-and-evaluation)
- [Perspective Papers](#perspective-papers)
- [Adversarial Attack and Defense for Image Retrieval](#adversarial-attack-and-defense-for-image-retrieval)
- [Other Resources](#other-resources)


## Adversarial Attack

### Classical Black-hat SEO (Spamming)
- [Web Spam Taxonomy.](http://ilpubs.stanford.edu:8090/771/1/2005-9.pdf) *Zoltan Gyongyi  et.al.* AIRWeb 2005.(**Web Spamming**)
- [International Workshop on Adversarial Information Retrieval on the Web.](http://www.ra.ethz.ch/cdstore/www2008/www2008.org/papers/pdf/p1267-castilloA.pdf)  AIRWeb 2005-2009.
- [Adversarial web search.](https://www.nowpublishers.com/article/DownloadSummary/INR-021) *Castillo, Carlos, and Brian D. Davison* FnTIR 2011.
- [MAWSEO: Adversarial Wiki Search Poisoning for Illicit Online Promotion.](https://arxiv.org/pdf/2304.11300.pdf) *Zilong Lin et.al.* S&P 2024. (**Adversarial Revisions**)

### White-hat SEO

- [Ranking-Incentivized Quality Preserving Content Modification.](https://arxiv.org/pdf/2005.12989) *Goren Gregory et.al.* SIGIR 2020.

### Neural Methods for IR Attack

- [One word at a time: adversarial attacks on retrieval models.](https://arxiv.org/pdf/2008.02197) *Raval, Nisarg, and Manisha Verma* Arxiv 2020.(**White-box**)
- [Adversarial Semantic Collisions.](https://arxiv.org/pdf/2011.04743) *Congzheng Song et.al.* EMNLP 2020.(**White-box**)
- [Bert rankers are brittle: A study using adversarial document perturbations.](https://arxiv.org/pdf/2206.11724) *Yumeng Wang et.al.* ICTIR 2022.(**White-box**)
- [PRADA: Practical Black-Box Adversarial Attacks against Neural Ranking Models.](https://arxiv.org/pdf/2204.01321) *Chen Wu et.al.* TOIS 2022.(**Black-box, Word substitution**)
- [Order-Disorder: Imitation Adversarial Attacks for Black-box Neural Ranking Models.](https://arxiv.org/pdf/2209.06506.pdf) *Jiawei Liu et.al.* CCS 2022.(**Black-box, Trigger**)
- [TRAttack: Text Rewriting Attack Against Text Retrieval](https://aclanthology.org/2022.repl4nlp-1.20.pdf) *Junshuai Song et.al.* RepL4NLP 2022. (**Rewriting Attack, Matching Model**)
- [Topic-oriented Adversarial Attacks against Black-box Neural Ranking Models.](https://arxiv.org/pdf/2304.14867.pdf) *Yu-An Liu et.al.* SIGIR 2023.(**Black-box, TARA task**)
- [Towards Imperceptible Document Manipulations against Neural Ranking Models.](https://arxiv.org/pdf/2305.01860.pdf) *Xuanang Chen et.al.* ACL 2023 findings.(**Black-box, Prompt**)
- [Black-box Adversarial Attacks against Dense Retrieval Models: A Multi-view Contrastive Learning Method](https://dl.acm.org/doi/pdf/10.1145/3583780.3614793) *Yu-An Liu et.al.* CIKM 2023.(**Black-box, Dense Retrieval Attack**)
- [Boosting Big Brother: Attacking Search Engines with Encodings.](https://arxiv.org/pdf/2304.14031.pdf) *Nicholas Boucher et.al.* RAID 2023.(**Encoding attack**)
- [Backdoor Attacks on Dense Passage Retrievers for Disseminating Misinformation.](https://arxiv.org/pdf/2402.13532.pdf) *Quanyu Long et.al.* Arxiv 2024.(**Backdoor attack**)
- [Poisoning Retrieval Corpora by Injecting Adversarial Passages.](https://arxiv.org/pdf/2402.13532.pdf) *Zexuan Zhong et.al.* EMNLP 2023.(**Dense Retrieval attack**)
- [Multi-granular Adversarial Attacks against Black-box Neural Ranking Models.](https://arxiv.org/pdf/2404.01574.pdf) *Yu-An Liu et.al.* SIGIR 2024.(**Multi-granular attack**)
- [Analyzing Adversarial Attacks on Sequence-to-Sequence Relevance Models.](https://arxiv.org/pdf/2403.07654.pdf) *Andrew Parry et.al.* ECIR 2024.(**Attacking T5**)

## Defense

### Adversarial Training

- [IRGAN: A Minimax Game for Unifying Generative and Discriminative Information Retrieval Models](https://arxiv.org/pdf/1705.10513) *Wang, Jun, et al.* SIGIR 2017.(**IRGAN**)
- [Adversarial Sampling and Training for Semi-Supervised Information Retrieval](https://arxiv.org/pdf/1811.04155) *Park, Dae Hoon, Yi Chang* WWW 2019.(**AdvIR**)
- [Adversarial Retriever-Ranker for dense text retrieval](https://arxiv.org/pdf/2110.03611) *Zhang, Hang, et al.* ICLR 2022.(**AR2**)
- [Towards Robust Ranker for Text Retrieval](https://arxiv.org/pdf/2206.08063.pdf) *Yucheng, Zhou, et al.* Arxiv 2022.(**R2ANKER**)
- [Dealing with textual noise for robust and effective BERT re-ranking](https://www.sciencedirect.com/science/article/pii/S0306457322002369) *Chen, Xuanang, et al.* IPM 2023.
- [A Study on FGSM Adversarial Training for Neural Retrieval](https://arxiv.org/pdf/2301.10576) *Lupart, Simon, Stéphane Clinchant* ECIR 2023.
- [Perturbation-Invariant Adversarial Training for Neural Ranking Models: Improving the Effectiveness-Robustness Trade-Off](https://ojs.aaai.org/index.php/AAAI/article/view/28730/29409) *Yu-An Liu et.al.* AAAI 2024.(**Perturbation-invariance theory**)

### Certified Defense

- [Certified Robustness to Word Substitution Ranking Attack for Neural Ranking Models](https://arxiv.org/pdf/2209.06691.pdf) *Chen Wu et.al.* CIKM 2022

### Detection

- [Defense of Adversarial Ranking Attack in Text Retrieval: Benchmark and Baseline via Detection](https://arxiv.org/pdf/2307.16816.pdf) *Xuanang Chen et.al.* Arxiv 2023

## Out-of-distribution

### Data Augmentation

* [Data augmentation for sample efficient and robust document ranking](https://dl.acm.org/doi/abs/10.1145/3634911) *Abhijit Anand et al.* TOIS 2023.
* [Data augmentation and transfer learning for brain tumor detection in magnetic resonance imaging](https://ieeexplore.ieee.org/abstract/document/9720964/)  *A. Anaya-Isaza et al.* IEEE Access 2022.
* [InPars: Data Augmentation for Information Retrieval using Large Language Models](https://arxiv.org/pdf/2202.05144.pdf) *Bonifacio et al.* Arxiv 2022.
* [HypeR: Multitask Hyper-Prompted Training Enables Large-Scale Retrieval Generalization](https://openreview.net/pdf?id=kUf4BcWXGJr) *Cai et al.* ICLR 2023.
* [DUQGen: Effective Unsupervised Domain Adaptation of Neural Rankers by Diversifying Synthetic Query Generation](https://arxiv.org/abs/2404.02489) *Ramraj Chandradevan et al.* Arxiv 2024.
* [Cross-domain augmentation networks for click-through rate prediction](https://arxiv.org/abs/2305.03953) *Xu Chen et al.* Arxiv 2023.(**CDAnet**)
* [Promptagator: Few-shot dense retrieval from 8 examples](https://arxiv.org/abs/2209.11755) *Zhuyun Dai et al.* Arxiv 2022.(**PROMPTAGATOR**)
* [Augmenting zero-shot dense retrievers with plug-in mixture-of-memories](https://arxiv.org/abs/2302.03754) *Suyu Ge et al.* EMNLP 2023.(**MoMA**)
* [Unsupervised dense information retrieval with contrastive learning](https://arxiv.org/abs/2112.09118) *Gautier Izacard et al.* Arxiv 2021. 
* [InRanker: Distilled Rankers for Zero-shot Information Retrieval](https://arxiv.org/abs/2401.06910) *Thiago Laitz et al.* Arxiv 2024. (**InRanker**)
* [Domain Adaptation for Dense Retrieval and Conversational Dense Retrieval through Self-Supervision by Meticulous Pseudo-Relevance Labeling](https://arxiv.org/abs/2403.08970) *Minghan Li and Eric Gaussier.* LREC-COLING 2024.(**DoDress**) 
* [Embedding-based zero-shot retrieval through query generation](https://arxiv.org/abs/2009.10270) *Davis Liang et al.* Arxiv 2020. 
* [Challenges in generalization in open domain question answering](https://arxiv.org/abs/2109.01156) *Linqing Liu et al.* NAACL 2022. 
* [Zero-shot neural passage retrieval via domain-targeted synthetic question generation ](https://arxiv.org/abs/2004.14503) *Ji Ma et al.* EACL 2021.
* [Text and code embeddings by contrastive pre-training](https://arxiv.org/abs/2201.10005) *Arvind Neelakantan et al.* Arxiv 2022.
* [Data augmentation for neural machine translation using generative language model](https://arxiv.org/abs/2307.16833) *Seokjin Oh et al.* Arxiv 2023.
* [Learning to retrieve passages without supervision](https://arxiv.org/abs/2112.07708) *Ori Ram et al.* NAACL 2022.(**Spider**)
* [Towards robust neural retrieval models with synthetic pre-training](https://arxiv.org/abs/2104.07800) *Revanth Gangi Reddy et al.* Arxiv 2021.
* [Questions are all you need to train a dense passage retriever](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00564/116466) *Devendra Singh Sachan et al.* TACL. (**ART**)
* [Beir: A heterogenous benchmark for zero-shot evaluation of information retrieval models](https://arxiv.org/abs/2104.08663) *Nandan Thakur et al.* NeurIPS 2021. (**BEIR**)
* [GPL: Generative pseudo labeling for unsupervised domain adaptation of dense retrieval](https://arxiv.org/abs/2112.07577) *Kexin Wang et al.* NAACL 2022. (**GPL**)
* * [Coco-dr: Combating distribution shifts in zero-shot dense retrieval with contrastive and distributionally robust learning ](https://arxiv.org/abs/2210.15212) Arxiv 2022. (**Coco-dr**)


### Domain Modeling

* [Coco-dr: Combating distribution shifts in zero-shot dense retrieval with contrastive and distributionally robust learning ](https://arxiv.org/abs/2210.15212) *Yu et al.* Arxiv 2022. (**Coco-dr**)
* [Improving Retrieval in Theme-specific Applications using a Corpus Topical Taxonomy](https://dl.acm.org/doi/abs/10.1145/3589334.3645512) *SeongKu Kang et al.* Arxiv 2024.(**ToTER**)
* [Learning list-level domain-invariant representations for ranking](https://proceedings.neurips.cc/paper_files/paper/2023/hash/cc473bb3ec4176a5e640c3a6b5fb5239-Abstract-Conference.html) *Ruicheng Xian et al.* NeurIPS 2023.
* [Zero-shot dense retrieval with momentum adversarial domain invariant representations](https://arxiv.org/abs/2110.07581) *Ji Xin et al.* ACL 2022. (**MoDIR**)
* [BERM: Training the balanced and extractable representation for matching to improve generalization ability of dense retrieval](https://arxiv.org/abs/2305.11052) *Shicheng Xu et al.* ACL 2023. (**BERM**)
* [Disentangled modeling of domain and relevance for adaptable dense retrieval](https://arxiv.org/abs/2208.05753) *Jingtao Zhan et al.* (**DDR**)

### Architectural Modifications

* [Out-of-domain semantics to the rescue! zero-shot hybrid retrieval models](https://link.springer.com/chapter/10.1007/978-3-030-99736-6_7) *Tao Chen et al.* ECIR 2022.
* [From distillation to hard negative sampling: Making sparse neural ir models more effective](https://dl.acm.org/doi/abs/10.1145/3477495.3531857) *Thibault Formal et al.* SIGIR 2022. 
* [Zero-shot retrieval with search agents and hybrid environments](https://arxiv.org/abs/2209.15469) *Michelle Chen Huebscher et al.* Arxiv 2022. 
* [DESIRE-ME: Domain-Enhanced Supervised Information Retrieval Using Mixture-of-Experts](https://link.springer.com/chapter/10.1007/978-3-031-56060-6_8) *Pranav Kasela et al.* ECIR 2024. (**DESIRE-ME**)
* [Back to Basics: A Simple Recipe for Improving Out-of-Domain Retrieval in Dense Encoders](https://arxiv.org/abs/2311.09765) *Hyunji Lee et al.* Arxiv 2023. 

### Scaling up the Model Capacity

* [Ernie-search: Bridging cross-encoder with dual-encoder via self on-the-fly distillation for dense passage retrieval](https://arxiv.org/abs/2205.09153) *Yuxiang Lu et al.* Arxiv 2022. 
* [Large dual encoders are generalizable retrievers](https://arxiv.org/abs/2112.07899) *Jianmo Ni et al.* EMNLP 2022. 

### Continual Learning for Generative Retrieval

* [Continual learning for generative retrieval over dynamic corpora](https://dl.acm.org/doi/abs/10.1145/3583780.3614821) *Jiangui Chen et al.* CIKM 2023. (**CLEVER**)
* [Corpusbrain++: A continual generative pre-training framework for knowledge-intensive language tasks](https://arxiv.org/abs/2402.16767) *Jiafeng Guo et al.* Arxiv 2024. (**CorpusBrain++**)
* [Incdsi: incrementally updatable document retrieval](https://proceedings.mlr.press/v202/kishore23a.html) *Varsha Kishore el al.* PMLR 2023. (**IncDSI**)
* [DSI++: Updating transformer memory with new documents](https://arxiv.org/abs/2212.09744) *Sanket Mehta et al.* EMNLP 2023. (**DSI++**)
* [Continually Updating Generative Retrieval on Dynamic Corpora](https://www.researchgate.net/publication/371163230_Continually_Updating_Generative_Retrieval_on_Dynamic_Corpora/fulltext/6476b927a25e543829dfebb1/Continually-Updating-Generative-Retrieval-on-Dynamic-Corpora.pdf?_tp=eyJjb250ZXh0Ijp7ImZpcnN0UGFnZSI6InB1YmxpY2F0aW9uIiwicGFnZSI6InB1YmxpY2F0aW9uIn19) *Soyoung Yoon et al.* Arxiv 2023. 

### Continual Learning for Dense Retrieval

* [L2R: Lifelong Learning for First-stage Retrieval with Backward-Compatible Representations](https://dl.acm.org/doi/abs/10.1145/3583780.3614947) *Yinqiong Cai et al.* CIKM 2023. (**L$^2$R**)

### Query Variations

- [Dealing with Typos for BERT-based Passage Retrieval and Ranking](https://arxiv.org/pdf/2108.12139) *Shengyao Zhuang et al.* EMNLP 2021.(**DRTA**)
- [Towards Robust Dense Retrieval via Local Ranking Alignment](https://www.ijcai.org/proceedings/2022/0275.pdf) *Xuanang Chen et al.* IJCAI 2022.(**RoDR**)
- [Evaluating the Robustness of Retrieval Pipelines with Query Variation Generators](https://arxiv.org/pdf/2111.13057) *Penha Gustavo et al.* ECIR 2022.
- [CharacterBERT and Self-Teaching for Improving the Robustness of Dense Retrievers on Queries with Typos](https://arxiv.org/pdf/2204.00716) *Shengyao Zhuang et al.* SIGIR 2022.(**CBST**)
- [Analysing the Robustness of Dual Encoders for Dense Retrieval Against Misspellings](https://arxiv.org/pdf/2205.02303) *Sidiropoulos Georgios et al.* SIGIR 2022.(**DACL**)
- [MIRS: [MASK] Insertion Based Retrieval Stabilizer for Query Variations](https://link.springer.com/chapter/10.1007/978-3-031-39847-6_31) *Junping Liu et al.* DEXA 2023.(**MIRS**)
- [Typos-aware bottlenecked pre-training for robust dense retrieval](https://arxiv.org/pdf/2304.08138) *Shengyao Zhuang et al.* SIGIR-AP 2023(**ToRoDer**)
- [Contrastive fine-tuning improves robustness for neural rankers](https://arxiv.org/abs/2105.12932) *Xiaofei Ma et al.* ACL-IJCNLP 2021.
- [Improving the Robustness of Dense Retrievers Against Typos via Multi-Positive Contrastive Learning](https://arxiv.org/pdf/2403.10939) *Georgios Sidiropoulos et al.* ECIR 2024.
- [Noise-robust dense retrieval via contrastive alignment post training](https://arxiv.org/abs/2304.03401) *Daniel Campos et al.* Arxiv 2023.(**CAPOT**)
- [Towards Robust Neural Rankers with Large Language Model: A Contrastive Training Approach](https://www.mdpi.com/2076-3417/13/18/10148) *Ziyang Pan et al.* Applied Sciences 2023.
- [Typo-robust representation learning for dense retrieval](https://arxiv.org/abs/2306.10348) *Panuthep Tasawong et al.* ACL 2023.(**DST**)

### Unseen Query Type

- [Learning to Jointly Transform and Rank Difficult Queries](https://link.springer.com/chapter/10.1007/978-3-031-56066-8_5) *Amin Bigdeli et al.* ECIR 2024.
- [Cross domain regularization for neural ranking models using adversarial learning](https://dl.acm.org/doi/abs/10.1145/3209978.3210141) *Daniel Cohen et al.* SIGIR 2018.
- [Ms-shift: An analysis of ms marco distribution shifts on neural retrieval](https://link.springer.com/chapter/10.1007/978-3-031-28244-7_40) *Simon Lupart at al.* ECIR 2023.(**MS-Shift**)
- [Contrastive fine-tuning improves robustness for neural rankers](https://arxiv.org/abs/2105.12932) *Xiaofei Ma et al.* ACL-IJCNLP 2021.
- [Simple entity-centric questions challenge dense retrievers](https://arxiv.org/abs/2109.08535) *Christopher Sciavolino et al.* EMNLP 2021.

## Benchmark and Evaluation

- [Are Neural Ranking Models Robust?](https://arxiv.org/pdf/2108.05018.pdf) *Chen Wu et.al.* TOIS 2022
- [Evaluating Interpolation and Extrapolation Performance of Neural Retrieval Models.](https://dl.acm.org/doi/pdf/10.1145/3511808.3557312) *Jingtao Zhan et.al.* CIKM 2022

## Perspective Papers

- [Competitive Search.](https://dl.acm.org/doi/pdf/10.1145/3477495.3532771) *Oren Kurland et.al.* SIGIR 2022.(**Competitive Search**)
- [A Game Theoretic Analysis of the Adversarial Retrieval Setting.](https://www.jair.org/index.php/jair/article/download/11104/26296) *Basat, Ran Ben et.al.* JAIR 2017.(**PRP is sub-optimal**)

## Adversarial Attack and Defense for Image Retrieval

- [Targeted Mismatch Adversarial Attack: Query with a Flower to Retrieve the Tower](http://openaccess.thecvf.com/content_ICCV_2019/papers/Tolias_Targeted_Mismatch_Adversarial_Attack_Query_With_a_Flower_to_Retrieve_ICCV_2019_paper.pdf) *Giorgos Tolias et al.* ICCV 2019.(**TMA**)
- [Universal Perturbation Attack Against Image Retrieval](https://openaccess.thecvf.com/content_ICCV_2019/papers/Li_Universal_Perturbation_Attack_Against_Image_Retrieval_ICCV_2019_paper.pdf) *Jie Li et al.* ICCV 2019.(**UAP**)
- [Adversarial Ranking Attack and Defense](https://arxiv.org/pdf/2002.11293) *Mo Zhou et al.* ECCV 2020.(**Candidate Attack and Query Attack**)
- [You See What I Want You to See: Exploring Targeted Black-Box Transferability Attack for Hash-based Image Retrieval Systems](https://openaccess.thecvf.com/content/CVPR2021/papers/Xiao_You_See_What_I_Want_You_To_See_Exploring_Targeted_CVPR_2021_paper.pdf) *Yanru Xiao et al.* CVPR 2021.(**Hash-based: Noise-induced Adversarial Generation**)
- [Practical Relative Order Attack in Deep Ranking](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhou_Practical_Relative_Order_Attack_in_Deep_Ranking_ICCV_2021_paper.pdf) *Mo Zhou et al.* ICCV 2021.
- [QAIR: Practical Query-efficient Black-Box Attacks for Image Retrieval](http://openaccess.thecvf.com/content/CVPR2021/papers/Li_QAIR_Practical_Query-Efficient_Black-Box_Attacks_for_Image_Retrieval_CVPR_2021_paper.pdf) *Xiaodan Li et al.* CVPR 2021.(**Query-based Attack against Image Retrieval**)
- [ARRA: Absolute-Relative Ranking Attack against Image Retrieval](https://dl.acm.org/doi/abs/10.1145/3503161.3548138) *Siyuan Li et al.* MM 2022.(**ARRA**)
- [RetrievalGuard: Provably Robust 1-Nearest Neighbor Image Retrieval](https://proceedings.mlr.press/v162/wu22o/wu22o.pdf) *Yihan Wu et al.* ICML 2022.(**RetrievalGuard**)

## Other Resources

- [CREDENCE: Counterfactual Explanations for Document Ranking](https://arxiv.org/pdf/2302.04983) *Rorseth Joel et al.* Arxiv 2023. [Webpage of interactive tool](http://lg-research-1.uwaterloo.ca:8091/credence/builder)







