# NLP Deeplearning PaperNote
####2017-2
ICLR 2017 Accpeted Paper I have read / am going to read [[ICLR](https://openreview.net/group?id=ICLR.cc/2017/conference)]

<li>A Compare-Aggregate Model for Matching Text Sequences. 实验很solid
<li>Dynamic Coattention Networks For Question Answering. DMN做阅读理解

####Language Model

<li>Pointer Sentinel Mixture Models. 开放了一个LM数据集，模型是PointerNetwork的延伸
<li>Frustratingly Short Attention Spans in Neural Language Modeling. 与以往attention不同的是，他把hidden分了三部分，分别是负责对齐的，负责hidden的和负责predict的（key,value, predict) 
<li>Improving Neural Language Models with a Continuous Cache 这篇paper的idea是个boarderline的idea，但是他中了。Cache For LSTM并不新颖。这篇文章的最大贡献是他把Copy Mechanism 加速了，实用，且效果好。我觉得Reviewer1给的Review非常非常的中肯，这篇文章更适合写NLP的会。
<li>DATA NOISING AS SMOOTHING IN NEURAL NETWORK LANGUAGE MODELS 文章把Ngram的平滑技术给RNN了，虽然写着感觉理论直观不强，但是引发了一个值得思考的问题，Ngram平滑是要区别对待stop word和非stop word，非stopword预测错了的惩罚更高，然而RNN没有这个，这导致了RNN在训练上把stop word的预测训练好，而放弃了低频词的预测。这也进一步引发了，类似于safe response在聊天中的出现。


End ICLR

<li>Wasserstein GAN[[ArXiv](https://arxiv.org/pdf/1701.06547)] 重剑无锋，大巧不工。用深度的数学理论推导出了简单易懂的GAN训练方法</li>
<li>Adversarial Learning for Neural Dialogue Generation[[ArXiv](https://arxiv.org/pdf/1701.06547)] 大哥确实动手快，感觉需要这篇paper的code~</li>
<li>DeepStack: Expert-Level Artificial Intelligence in No-Limit Poker[[ArXiv](https://arxiv.org/abs/1701.01724)] 这篇论文的AI可以平局每局赢450mbb，至少可以拿来赚钱了</li>
<li>DyNet: The Dynamic Neural Network Toolkit [[ArXiv](https://arxiv.org/pdf/1701.03980.pdf)] 知情人士表示，在很多种情况下TF比DyNet快</li>


####2016-12

<li>Language Modeling with Gated Convolutional Networks[[ArXiv](https://arxiv.org/abs/1612.08083)]如果说有什么亮眼的可能是快。。。</li>

<li>Sequential Match Network: A New Architecture for Multi-turn Response Selection in Retrieval-based Chatbots [[ArXiv](https://arxiv.org/abs/1612.01627)]</li>

<li>Learning Through Dialogue Interactions [[ArXiv](https://arxiv.org/abs/1612.04936)]</li>

<li>A Simple, Fast Diverse Decoding Algorithm for Neural Generation[[ArXiv](https://arxiv.org/abs/1611.08562)]</li>

