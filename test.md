### All About Padding & Pooling in CNN ###
+ Deep learning is _ALL ABOUT SHRINK DIMS_
+ In the shrinking if we foucd on middle but not conner   
Things will go bad THAT WE USING PADDING
+ MaxPooing is proved to functional _BUNT DO NOT KNOW WHY_

#### Conv2d ####
+ stride
    >>> m = nn.Conv2d(16, 33, 3, stride=2)  
    >>> m = nn.Conv2d(16, 33, (3, 5), stride=(2, 1), padding=(4, 2))  
    >>> m = nn.Conv2d(16, 33, (3, 5), stride=(2, 1), padding=(4, 2), dilation=(3, 1))  
    >>> input = torch.randn(20, 16, 50, 100)  
    >>> output = m(input)  

### Batchnorm  Layernorm ###
 + standard 
   + Batchnorm in CV tasks & Layernorm in NLP tasks.
+ VGG's normalisation is layer normalisation???
>>> How to use _batch_ normalisation & _layer_ normalisation???



### TextCNN ###

#### Channel_input ####

+ 输入的channel通常是不同方式的embedding方式（比如 word2vec或Glove）
+ 利用静态词向量和fine-tunning词向量作为不同channel的做法。
  + 静态(static)方式：训练过程中不再更新embeddings。实质上属于迁移学习，特别是在目标领域数据量比较小的情况下，采用静态的词向量效果也不错。（通过设置trainable=False）
  + 非静态(non-static)方式：在训练过程中对embeddings进行更新和微调(fine tune)，能加速收敛。（通过设置trainable=True）
  
#### Channel_output ####
+ usually 2

