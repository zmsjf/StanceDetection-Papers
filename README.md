# StanceDetection-Papers
不同数据集上的工作
跨target工作，纯立场检测，引入数据

## Reference
**[summarization.bib]**(https://github.com/zmsjf/StanceDetection-Papers/blob/main/summrization.bib)

## Benchmark
1. **SemEval-2016 Task 6: Detecting Stance in Tweets** *Saif M. Mohammad,Svetlana Kiritchenko,Parinaz Sobhani,Xiaodan Zhu,Colin Cherry* [[pdf]](https://aclanthology.org/S16-1003.pdf)  
2. **Overview of NLPCC Shared Task 4: Stance Detection in Chinese Microblogs**![](https://img.shields.io/badge/-Chinese-orange)*Ruifeng Xu,Jiachen Du,Lin Gui*[[pdf]](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/NLPCC2016OverviewofStnaceDetection%20(2).pdf)
3. **FNC-1**(https://github.com/FakeNewsChallenge/fnc-1)
4. **RumourEval**(https://alt.qcri.org/semeval2017/task8/)

## Stance Detection work
|ID|Name|Description|Dataset|Paper|Conference|
|:---:|:---:|:---:|:---:|:---:|:---:|
|1|[X]|-|从procon.org整理数据。引入sentiment、emotion信息。bert拿到结果之后，不直接进行分类，又利用GRU和max-pool和avg-pool进行表示|[Stance Prediction for Contemporary Issues: Data and Experiments](https://aclanthology.org/2020.socialnlp-1.5.pdf)|ACL20|
|2|[X]|-|-|[Stance Prediction and Claim Verification: An Arabic Perspective](https://aclanthology.org/2020.fever-1.2.pdf)|ACL20|
|3|[X]|-|-|[Agreement Prediction of Arguments in Cyber Argumentation for Detecting Stance Polarity and Intensity](https://aclanthology.org/2020.acl-main.509.pdf)|ACL20|
|4|[X]|-|-|[Enhancing Cross-target Stance Detection with Transferable Semantic-Emotion Knowledge](https://aclanthology.org/2020.acl-main.291.pdf)|ACL20|
|5|[X]|-|构建twitter数据集|[Will-They-Won’t-They: A Very Large Dataset for Stance Detection on Twitter](https://aclanthology.org/2020.acl-main.157.pdf)|ACL20|
|6|[X]|-|-|[Predicting the Topical Stance and Political Leaning of Media using Tweets](https://aclanthology.org/2020.acl-main.50.pdf)|ACL20|
|7|[SCN]|立场并不是互相独立的，需要单独学习每个立场，考虑立场之间的相关性|SemEval taskA|[Stance Detection with Stance-Wise Convolution Network](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Stance%20Detection%20with%20Stance-Wise%20Convolution%20Network.pdf)|NLPCC20|
|8|[CKEMN]|引入ConceptNet知识，帮助丰富text和target的上下文|SemEval16 taskA|[Commonsense Knowledge Enhanced Memory Network for Stance Classification](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Commonsense%20Knowledge%20Enhanced%20Memory%20Network%20for%20Stance%20Classification.pdf)|IEEE20|
|8|[PNEM]|使用densely connected Bi-LSTM和 nested LSTMs architectures和注意力机制|SemEval taskA,Multi-target|[Tweet Stance Detection Using an Attention based Neural Ensemble Model](https://aclanthology.org/N19-1185.pdf)|NAACL19|
|7|[stancy]|bert,加入cos约束|Perspectrum dataset|[STANCY: Stance Classification Based on Consistency Cues](https://aclanthology.org/D19-1675.pdf)|EMNLP19|
|8|[MTransSAN]|多任务，Sentiment Analysis,QA,Textual Entailment,Paraphrase Detection。基本思想：在四个任务上用任务语料进行预训练，再用FNC-1语料进行fine-tuning|FNC-1|[Neural Multi-Task Learning for Stance Prediction](https://aclanthology.org/D19-6603.pdf)|EMNLP19|
|9|[X]|-|BBC,ETC(tweet),MFTC(tweet)|[Incorporating Label Dependencies in Multilabel Stance Detection](https://aclanthology.org/D19-1665.pdf)|EMNLP19|
|10|[X]|多任务(待看)|SemEval taskA|[Multi-Task Stance Detection with Sentiment and Stance Lexicons](https://aclanthology.org/D19-1657.pdf)|EMNLP19|
|11|[CLMN]|跨语言|FNC-1|[Contrastive Language Adaptation for Cross-Lingual Stance Detection](https://aclanthology.org/D19-1452.pdf)|EMNLP19|
|12|[X]|-|RumourEval,FNC-1|[Gradual Argumentation Evaluation for Stance Aggregation in Automated Fake News Detection](https://aclanthology.org/W19-4518.pdf)|ACL19|
|13|[X]|-|数据集|[Data Set for Stance and Sentiment Analysis from User Comments on Croatian News](https://aclanthology.org/W19-3707.pdf)|ACL19|
|14|[X]|-|Pheme 5 events dataset|[Tree LSTMs with Convolution Units to Predict Stance and Rumor Veracity in Social Media Conversations](https://aclanthology.org/P19-1498.pdf)|ACL19|
|15|[X]|-|-|[Recognising Agreement and Disagreement between Stances with ReasonComparing Networks](https://aclanthology.org/P19-1460.pdf)|ACL19|
|19|[AEKFW]|从twitter，wikipedia构建数据集，在立场检测模型中加入Wikipedia信息，设定关系为pro，sup，proby，supby|[Stance Detection Attending External Knowledge from Wikipedia](https://www.jstage.jst.go.jp/article/ipsjjip/27/0/27_499/_pdf/-char/en)|IPSJ19|
|16|[X]|加入用户信息|SemEval taskA，Gun（自己）|[Using Author Embeddings to Improve Tweet Stance Classification](https://aclanthology.org/W18-6124/)|EMNLP18|
|17|[X]|-|FNC-1|[Stance Detection in Fake News: A Combined Feature Representation](https://aclanthology.org/W18-5510.pdf)|EMNLP18|
|18|[X]|-|FNC-1|[Towards Automatic Fake News Detection: Cross-Level Stance Detection in News Articles](https://aclanthology.org/W18-5507.pdf)|EMNLP18|
|19|[CrossNet]|跨target|SemEval2016 taskA|[Cross-Target Stance Classification with Self-Attention Networks](https://aclanthology.org/P18-2123.pdf)|ACL18|
|20|[X]|-|-|[A Retrospective Analysis of the Fake News Challenge Stance-Detection Task](https://aclanthology.org/C18-1158.pdf)|COLING18|
|21|[X]|-|-|[Structured Representation Learning for Online Debate Stance Prediction](https://aclanthology.org/C18-1316.pdf)|COLING18|
|22|[X]|-|-|[Predicting Stances from Social Media Posts using Factorization Machines](https://aclanthology.org/C18-1286.pdf)|COLING18|
|23|[HAN]|-|SemEval16 taskA,H&N14|[Stance Detection with Hierarchical Attention Network](https://aclanthology.org/C18-1203.pdf)|COLING18|
|24|[X]|-|-|[ConStance: Modeling Annotation Contexts to Improve Stance Classification](https://aclanthology.org/D17-1116/)|EMNLP2017|
|26|[TAN]|在模型层面注意到target|SemEval16 taskA,NLPCC16 taskA|[Stance Classification with Target-Specific Neural Attention Networks](https://www.ijcai.org/proceedings/2017/0557.pdf)|IJCAI17|
|25|[BiCond]| 经典 |SemEval taskB|[Stance Detection with Bidirectional Conditional Encoding](https://aclanthology.org/D16-1084/)|EMNLP2016|
|26|[X]|-|-|[Weakly Supervised Tweet Stance Classification by Relational Bootstrapping](https://aclanthology.org/D16-1105/)|EMNLP2016|
|27|[X]|-|-|[Modeling Stance in Student Essays](https://aclanthology.org/P16-1205.pdf)|ACL16|
|28|[X]|-|-|[Hawkes Processes for Continuous Time Sequence Classification: an Application to Rumour Stance Classification in Twitter](https://aclanthology.org/P16-2064.pdf)|ACL16|
|29|[STS]|不是深度学习方法，概率|SemEval taskA&B|[A Joint Sentiment-Target-Stance Model for Stance Classification in Tweets](https://aclanthology.org/C16-1250.pdf)|COLING16|
|30|[X]|-|PHEME rumour|[Stance Classification in Rumours as a Sequential Task Exploiting the Tree Structure of Social Media Conversations](https://aclanthology.org/C16-1230.pdf)|COLING16|
|31|[UTCNN]|-|FBFans(中文),CreateDebate|[UTCNN: a Deep Learning Model of Stance Classification on Social Media Text](https://aclanthology.org/C16-1154.pdf)|COLING16|
|39|[pkudblab]|SemEval 2016 taskA第二名，taskB第一名。利用CNN和投票策略。对五个target单独训练五个模型|SemEval taskA&B|[pkudblab at SemEval-2016 Task 6 : A Specific Convolutional Neural Network System for Effective Stance Detection](https://aclanthology.org/S16-1062.pdf)|SemEval16|









