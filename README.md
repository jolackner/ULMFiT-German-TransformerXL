# TransformerXL German Wikipedia Language Model 
- vocabulary size = 60,000
- trained on 100 million words collected from German Wikipedia (equivalent to 10% of all articles containing more than 1000 charactes)
- perplexity of best validation loss: 18.9, **but**:
- 6.5% OOV/Out Of Vocabulary in Train Set, 6.9% OOV in Valid Set seems a high percentage, making low valid loss & perplexity less meaningful
- mem_len= 50 (reduced length, to shorten training time)

- adapted from Cristian Duguet's [Spanish ULMFiT Language Model][duguet]
- using hyperparameters suggested by [Kaspar Lund][lund] 
- trained with the great [fastai][linkfastai] library 
- Download [itos file][linkitos] and [weights][linkweights] of last epoch. 

[linkitos]: <https://drive.google.com/file/d/14cp8dH8aOm97g_O474Cl-mvjAZJjtGa_/view?usp=sharing>
[linkweights]: <https://drive.google.com/open?id=1eSwOWT-vkKyUuyYO1BU8M-ZoXXE81WJp>
[linkfastai]: <http://docs.fast.ai>
[lund]: <https://forums.fast.ai/t/training-transformerxl/40104>
[duguet]: <https://github.com/cduguet/ulmfit-es/blob/master/ULMFit-TransfXL.ipynb>
