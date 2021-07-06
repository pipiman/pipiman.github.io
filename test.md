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
>>> How to use batch normalisation & layer normalisation???
