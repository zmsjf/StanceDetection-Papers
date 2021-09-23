# StanceDetection-Papers

## Literature Review
**Stance Detection: A Survey** *DILEK KÜÇÜK,FAZLI CAN*`ACM19`[[pdf]](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Stance%20Detection%20A%20Survey.pdf)

## Dataset
1. **SemEval-2016 Task 6: Detecting Stance in Tweets** *Saif M. Mohammad,Svetlana Kiritchenko,Parinaz Sobhani,Xiaodan Zhu,Colin Cherry* [[pdf]](https://aclanthology.org/S16-1003.pdf)  
2. **A Dataset for Multi-Target Stance Detection**(pair-target) [[pdf]](https://aclanthology.org/E17-2088.pdf)
3. **Overview of NLPCC Shared Task 4: Stance Detection in Chinese Microblogs**![](https://img.shields.io/badge/-Chinese-orange)*Ruifeng Xu,Jiachen Du,Lin Gui*[[pdf]](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/NLPCC2016OverviewofStnaceDetection%20(2).pdf)
4. **FNC-1**(https://github.com/FakeNewsChallenge/fnc-1)
5. **RumourEval**(https://alt.qcri.org/semeval2017/task8/)

## Stance Detection work
|ID|Name|Description|Dataset|Paper|Conference|
|:---:|:---:|:---:|:---:|:---:|:---:|
|1|[s/e-GRU]|引入sentiment、emotion信息。bert拿到结果之后，不直接进行分类，又利用GRU和max-pool和avg-pool进行表示|从procon.org整理数据。|[Stance Prediction for Contemporary Issues: Data and Experiments](https://aclanthology.org/2020.socialnlp-1.5.pdf)|ACL20|
|2|[X]|-|-|[Stance Prediction and Claim Verification: An Arabic Perspective](https://aclanthology.org/2020.fever-1.2.pdf)|ACL20|
|3|[X]|-|-|[Agreement Prediction of Arguments in Cyber Argumentation for Detecting Stance Polarity and Intensity](https://aclanthology.org/2020.acl-main.509.pdf)|ACL20|
|4|[X]|-|-|[Enhancing Cross-target Stance Detection with Transferable Semantic-Emotion Knowledge](https://aclanthology.org/2020.acl-main.291.pdf)|ACL20|
|5|[X]|在本文中，我们提出了一种级联方法，该方法使用无监督学习来利用Twitter用户的转发行为来确定其对两极分化话题的态度。 然后，它使用基于用户标签的监督学习来表征在线媒体和受欢迎的Twitter用户的一般政治倾向，以及他们对目标两极分化话题的立场。|构建twitter数据集|[Will-They-Won’t-They: A Very Large Dataset for Stance Detection on Twitter](https://aclanthology.org/2020.acl-main.157.pdf)|ACL20|
|6|[X]||自己构造的数据集|[Predicting the Topical Stance and Political Leaning of Media using Tweets](https://aclanthology.org/2020.acl-main.50.pdf)|ACL20|
|7|[SCN]|立场并不是互相独立的，需要单独学习每个立场，考虑立场之间的相关性|SemEval taskA|[Stance Detection with Stance-Wise Convolution Network](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Stance%20Detection%20with%20Stance-Wise%20Convolution%20Network.pdf)|NLPCC20|
|8|[CKEMN]|引入ConceptNet知识，帮助丰富text和target的上下文|SemEval16 taskA|[Commonsense Knowledge Enhanced Memory Network for Stance Classification](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Commonsense%20Knowledge%20Enhanced%20Memory%20Network%20for%20Stance%20Classification.pdf)|IEEE20|
|9|[PNEM]|使用densely connected Bi-LSTM和 nested LSTMs architectures和注意力机制|SemEval taskA,Multi-target|[Tweet Stance Detection Using an Attention based Neural Ensemble Model](https://aclanthology.org/N19-1185.pdf)|NAACL19|
|10|[stancy]|bert,加入cos约束|Perspectrum dataset|[STANCY: Stance Classification Based on Consistency Cues](https://aclanthology.org/D19-1675.pdf)|EMNLP19|
|11|[MTransSAN]|多任务，Sentiment Analysis,QA,Textual Entailment,Paraphrase Detection。基本思想：在四个任务上用任务语料进行预训练，再用FNC-1语料进行fine-tuning|FNC-1|[Neural Multi-Task Learning for Stance Prediction](https://aclanthology.org/D19-6603.pdf)|EMNLP19|
|12|[X]|-|BBC,ETC(tweet),MFTC(tweet)|[Incorporating Label Dependencies in Multilabel Stance Detection](https://aclanthology.org/D19-1665.pdf)|EMNLP19|
|13|[X]|多任务(待看)|SemEval taskA|[Multi-Task Stance Detection with Sentiment and Stance Lexicons](https://aclanthology.org/D19-1657.pdf)|EMNLP19|
|14|[CLMN]|跨语言|FNC-1|[Contrastive Language Adaptation for Cross-Lingual Stance Detection](https://aclanthology.org/D19-1452.pdf)|EMNLP19|
|15|[X]|-|RumourEval,FNC-1|[Gradual Argumentation Evaluation for Stance Aggregation in Automated Fake News Detection](https://aclanthology.org/W19-4518.pdf)|ACL19|
|16|[X]|-|数据集|[Data Set for Stance and Sentiment Analysis from User Comments on Croatian News](https://aclanthology.org/W19-3707.pdf)|ACL19|
|17|[X]|-|Pheme 5 events dataset|[Tree LSTMs with Convolution Units to Predict Stance and Rumor Veracity in Social Media Conversations](https://aclanthology.org/P19-1498.pdf)|ACL19|
|18|[X]|-|-|[Recognising Agreement and Disagreement between Stances with ReasonComparing Networks](https://aclanthology.org/P19-1460.pdf)|ACL19|
|19|[AEKFW]|在立场检测模型中加入Wikipedia信息，设定关系为pro，sup，proby，supby|从twitter，wikipedia构建数据集|[Stance Detection Attending External Knowledge from Wikipedia](https://www.jstage.jst.go.jp/article/ipsjjip/27/0/27_499/_pdf/-char/en)|IPSJ19|
|20|[RCA]|QA类型的立场检测|自己从Baidu Knows，Sogou Wenwen和Mingyi构建数据集|[Exploring Answer Stance Detection with Recurrent Conditional Attention](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Exploring%20Answer%20Stance%20Detection%20with%20Recurrent%20Conditional%20Attention.pdf)|AAAI19|
|21|[X]|-|-|[Modeling Transferable Topics for Cross-Target Stance Detection]()|SIGIR19|
|22|[AE-RNN]|在GRU基础上加入tweet用户信息。引入作者的知识改善推文立场分类，由于作者信息嵌入通常不适用于带标签的，所以提出半监督式预训练方法来预测用户嵌入|SemEval taskA，Gun（论文自己构建）|[Using Author Embeddings to Improve Tweet Stance Classification](https://aclanthology.org/W18-6124/)|EMNLP18|
|23|[X]|-|FNC-1|[Stance Detection in Fake News: A Combined Feature Representation](https://aclanthology.org/W18-5510.pdf)|EMNLP18|
|24|[X]|-|FNC-1|[Towards Automatic Fake News Detection: Cross-Level Stance Detection in News Articles](https://aclanthology.org/W18-5507.pdf)|EMNLP18|
|25|[CrossNet]|跨target|SemEval2016 taskA|[Cross-Target Stance Classification with Self-Attention Networks](https://aclanthology.org/P18-2123.pdf)|ACL18|
|26|[X]|-|-|[A Retrospective Analysis of the Fake News Challenge Stance-Detection Task](https://aclanthology.org/C18-1158.pdf)|COLING18|
|27|[X]|-|-|[Structured Representation Learning for Online Debate Stance Prediction](https://aclanthology.org/C18-1316.pdf)|COLING18|
|28|[X]|-|《Other topics you may also agree or disagree: Modeling inter-topic preferences using tweets and matrix factorization》|[Predicting Stances from Social Media Posts using Factorization Machines](https://aclanthology.org/C18-1286.pdf)|COLING18|
|29|[HAN]|引入Sentiment，Dependency，Argument，用注意力机制共同做立场检测|SemEval16 taskA,H&N14|[Stance Detection with Hierarchical Attention Network](https://aclanthology.org/C18-1203.pdf)|COLING18|
|30|[X]|-|-|[ConStance: Modeling Annotation Contexts to Improve Stance Classification](https://aclanthology.org/D17-1116/)|EMNLP17|
|31|[TAN]|在模型层面注意到target|SemEval16 taskA,NLPCC16 taskA|[Stance Classification with Target-Specific Neural Attention Networks](https://www.ijcai.org/proceedings/2017/0557.pdf)|IJCAI17|
|32|[BiCond]| 经典 |SemEval taskB|[Stance Detection with Bidirectional Conditional Encoding](https://aclanthology.org/D16-1084/)|EMNLP16|
|33|[X]|-|SemEval taskB|[Weakly Supervised Tweet Stance Classification by Relational Bootstrapping](https://aclanthology.org/D16-1105/)|EMNLP16|
|34|[X]|-|-|[Modeling Stance in Student Essays](https://aclanthology.org/P16-1205.pdf)|ACL16|
|35|[X]|-|-|[Hawkes Processes for Continuous Time Sequence Classification: an Application to Rumour Stance Classification in Twitter](https://aclanthology.org/P16-2064.pdf)|ACL16|
|36|[STS]|不是深度学习方法，概率|SemEval taskA&B|[A Joint Sentiment-Target-Stance Model for Stance Classification in Tweets](https://aclanthology.org/C16-1250.pdf)|COLING16|
|37|[X]|-|PHEME rumour|[Stance Classification in Rumours as a Sequential Task Exploiting the Tree Structure of Social Media Conversations](https://aclanthology.org/C16-1230.pdf)|COLING16|
|38|[UTCNN]|-|FBFans(中文),CreateDebate|[UTCNN: a Deep Learning Model of Stance Classification on Social Media Text](https://aclanthology.org/C16-1154.pdf)|COLING16|
|39|[]|-|-|[Stance Classification by Recognizing Related Events about Targets](https://ieeexplore.ieee.org/document/7817117?signout=success)|IEEE16|
|40|[pkudblab]|SemEval 2016 taskA第二名，taskB第一名。利用CNN和投票策略。对五个target单独训练五个模型|SemEval taskA&B|[pkudblab at SemEval-2016 Task 6 : A Specific Convolutional Neural Network System for Effective Stance Detection](https://aclanthology.org/S16-1062.pdf)|SemEval16|

## Cross-Target Stance Detection
1. **Enhancing Cross-target Stance Detection with Transferable Semantic-Emotion Knowledge** *Bowen Zhang, Min Yang, Xutao Li, Yunming Ye, Xiaofei Xu, Kuai Dai*`ACL20`[[pdf]](https://aclanthology.org/2020.acl-main.291.pdf)
2. **Cross-Target Stance Classification with Self-Attention Networks** *Chang Xu,Cecile Paris,Surya Nepal,Ross Sparks* `ACL18` [[pdf]](https://aclanthology.org/P18-2123.pdf)
3. **Modeling Transferable Topics for Cross-Target Stance Detection** *Penghui Wei,Wenji Mao* `SIGIR19` [[pdf]](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Modeling%20Transferable%20Topics%20for%20Cross-Target%20Stance%20Detection.pdf)

## Cross-Lingual
1. **Contrastive Language Adaptation for Cross-Lingual Stance Detection** *Mitra Mohtarami,James Glass,Preslav Nakov* `EMNLP19` [[pdf]](https://aclanthology.org/D19-1452.pdf)


## Commonsense Konwledge
1. **Commonsense Knowledge Enhanced Memory Network for Stance Classification** *Jiachen Du,Lin Gui,Ruifeng Xu,Yunqing Xia,Xuan Wang* `IEEE20`[[pdf]](https://github.com/zmsjf/StanceDetection-Papers/blob/main/slides/paper-slides/Commonsense%20Knowledge%20Enhanced%20Memory%20Network%20for%20Stance%20Classification.pdf)
2. **Stance Detection Attending External Knowledge from Wikipedia** *Kazuaki Hanawa,Akira Sasaki,Naoaki Okazaki,Kentaro Inui* `IPSJ19`[[pdf]](https://www.jstage.jst.go.jp/article/ipsjjip/27/0/27_499/_pdf/-char/en)


## Reference
**[summarization.bib]**(https://github.com/zmsjf/StanceDetection-Papers/blob/main/summrization.bib)




