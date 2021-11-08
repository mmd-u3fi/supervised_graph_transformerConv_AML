# Supervised Graph Transformer for Money Laundering Detection
This notebook demonstrates the potential of graph transformer architecture for detecting suspicious accounts based on their transactions.
Dataset is a synthetic transactions graph made by AMLSIM. 

Dataset consists of ~ 800k Transactions and 20k Accounts
                    
Network is trained to classify ndoes based on their transactional behavior into Suspicious (Fraud) or Normal

# Network Architecture:

TransformerConv(1, 64, heads=3)

TransformerConv(192, 64, heads=3)

Linear(in_features=192, out_features=32, bias=True)

Linear(in_features=32, out_features=2, bias=True)

# Free Parameters
157154
