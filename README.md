# TransformerXL German Wikipedia Language Model Test 
- vocabulary size = 60,000
- trained on 100 million words collected from German Wikipedia (equivalent to 10% of all articles containing more than 1000 charactes)
- perplexity of best validation loss: 18.9, **but**:
- 6.5% OOV/Out Of Vocabulary in Train Set, 6.9% OOV in Valid Set seems a high percentage, making low valid loss & perplexity less meaningful)
- mem_len= 50 (reduced length, to shorten training time)
- trained with the great fastai library: http://docs.fast.ai

- adapted from Christian Duguet's Spanish Language Model:
- https://github.com/cduguet/ulmfit-es/blob/master/ULMFit-TransfXL.ipynb
- using hpyerparameters suggested by Kaspar Lund: https://forums.fast.ai/t/training-transformerxl/40104
