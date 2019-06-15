import torch
import numpy as np

def mask_softmax(attention_score,X_len):
    maxlen = X.size(1)
    mask = torch.arange(maxlen)[None, :] < X_len[:, None]
    attention_score[~mask] = float('-inf')
    return torch.softmax(attention_score,dim=1)
