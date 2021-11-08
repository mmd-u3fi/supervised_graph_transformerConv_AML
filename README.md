# Supervised Graph Transformer for Money Laundering Detection
This notebook demonstrates the potential of graph transformer architecture for detecting suspicious accounts based on their transactions.
Dataset is a synthetic transactions graph made by AMLSIM. 
Network is trained to classify ndoes based on their transactional behavior into Suspicious (Fraud) or Normal

# Dataset
~800k Transactions

20k Accounts

# Network Architecture:

  * TransformerConv(1, 64, heads=3) # 1 node feature, node embedding size of 64 and 3 attention heads
  * TransformerConv(192, 64, heads=3) # 64 * 3 head input dim, new embedding size of 64
  * Linear(192, 32)
  * Linear(32, 2)

Transformer Layers also have a 4d input for edge_attr tensor

# Free Parameters
157154
