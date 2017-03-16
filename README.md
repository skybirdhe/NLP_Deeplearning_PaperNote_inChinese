# NLP Deeplearning PaperNote

#### 2017-2
ICLR 2017 Accpeted Paper I have read / am going to read [[ICLR](https://openreview.net/group?id=ICLR.cc/2017/conference)]

#### QA and Machine Comprehension
<li>A Compare-Aggregate Model for Matching Text Sequences. 实验很solid..不过现在这个文本匹配也是做不出啥新的东西了。
<li>Dynamic Coattention Networks For Question Answering. DMN做阅读理解
<li>Bidirectional Attention Flow for Machine Comprehension 又一篇阅读理解，融合了点char的信息
<li>Machine Comprehension Using Match-LSTM and Answer Pointer 第一篇做阅读理解的
说到阅读理解这个任务，这篇文章算是第一个刷Squad的，然而数字不太理想。不过之后的工作基本都是在他的框架下做，我觉得这个人任务现在逐渐变成了在框架下做，然后开始把每个模块细调，看Gain。。很难有surprising的模型，但总是有surprising的结果。我们叫这个 阅读理解 NN调参大作战好了~

#### Language Model

<li>Pointer Sentinel Mixture Models. 开放了一个LM数据集，模型是PointerNetwork的延伸
<li>Frustratingly Short Attention Spans in Neural Language Modeling. 与以往attention不同的是，他把hidden分了三部分，分别是负责对齐的，负责hidden的和负责predict的（key,value, predict) 
<li>Improving Neural Language Models with a Continuous Cache 这篇paper的idea是个boarderline的idea，但是他中了。Cache For LSTM并不新颖。这篇文章的最大贡献是他把Copy Mechanism 加速了，实用，且效果好。我觉得Reviewer1给的Review非常非常的中肯，这篇文章更适合写NLP的会。
<li>DATA NOISING AS SMOOTHING IN NEURAL NETWORK LANGUAGE MODELS 文章把Ngram的平滑技术给RNN了，虽然写着感觉理论直观不强，但是引发了一个值得思考的问题，Ngram平滑是要区别对待stop word和非stop word，非stopword预测错了的惩罚更高，然而RNN没有这个，这导致了RNN在训练上把stop word的预测训练好，而放弃了低频词的预测。这也进一步引发了，类似于safe response在聊天中的出现。

#### Attention Model
<li>A STRUCTURED SELF-ATTENTIVE SENTENCE EMBEDDING. 这篇文章提出了一个很简单，但是有一些道理的idea。每个词attent其他词的权重应该有多个而不是一个，所以attention vector在他这里就变成了matrix。之后利用penalize term对这个矩阵做了redundancy惩罚，让attention的权重分散。他做的是setence embedding,不过也可以扩展到其他领域。我认为这个idea非常值得一试。
<li> STRUCTURED ATTENTION NETWORKS  现在的attention机制是soft attention，我们仍然可以尝试hard attention，以及linear-chain的attention。我觉得这个论文拍NLP任务是很有道理的。



End ICLR
#### 2017-1
<li>Wasserstein GAN[[ArXiv](https://arxiv.org/pdf/1701.06547)] 重剑无锋，大巧不工。用深度的数学理论推导出了简单易懂的GAN训练方法</li>
<li>Adversarial Learning for Neural Dialogue Generation[[ArXiv](https://arxiv.org/pdf/1701.06547)] 大哥确实动手快，感觉需要这篇paper的code~</li>
<li>DeepStack: Expert-Level Artificial Intelligence in No-Limit Poker[[ArXiv](https://arxiv.org/abs/1701.01724)] 这篇论文的AI可以平局每局赢450mbb，至少可以拿来赚钱了</li>
<li>DyNet: The Dynamic Neural Network Toolkit [[ArXiv](https://arxiv.org/pdf/1701.03980.pdf)] 知情人士表示，在很多种情况下TF比DyNet快</li>


#### 2016-12

<li>Language Modeling with Gated Convolutional Networks[[ArXiv](https://arxiv.org/abs/1612.08083)]如果说有什么亮眼的可能是快。。。</li>

<li>Sequential Match Network: A New Architecture for Multi-turn Response Selection in Retrieval-based Chatbots [[ArXiv](https://arxiv.org/abs/1612.01627)]</li>

<li>Learning Through Dialogue Interactions [[ArXiv](https://arxiv.org/abs/1612.04936)]</li>

<li>A Simple, Fast Diverse Decoding Algorithm for Neural Generation[[ArXiv](https://arxiv.org/abs/1611.08562)]</li>

