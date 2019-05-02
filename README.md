# TransformerXL German Wikipedia Language Model 
- vocabulary size = 60,000
- trained on 100 million words collected from German Wikipedia (equivalent to 10% of all articles containing more than 1000 charactes)
- perplexity of best validation loss: 18.9, **but**:
- 6.5% OOV/Out Of Vocabulary in Train Set, 6.9% OOV in Valid Set seems a high percentage, making low valid loss & perplexity less meaningful
- mem_len= 50 (reduced length, to shorten training time)

- adapted from Christian Duguet's [Spanish ULMFiT Language Model][duguet]
- using hyperparameters suggested by [Kaspar Lund][lund] 
- trained with the great [fastai][linkfastai] library 


[linkfastai]: <http://docs.fast.ai>
[lund]: <https://forums.fast.ai/t/training-transformerxl/40104>
[duguet]: <https://github.com/cduguet/ulmfit-es/blob/master/ULMFit-TransfXL.ipynb>
