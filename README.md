# DMNAG_GaoJiajie
DMNAG graph neural network method for potential disease-metabolite associations prediction

# DMNAG for disease-metabolite associations prediction

# Dependecies
- Python 3.10.9
- pytorch 2.0.0
- numpy 1.23.5
- pandas 1.5.3
- scikit-learn 1.3.0


## Dataset
disease-metabolite associations: A.csv
Metabolite Node similarity features: MPCS.csv
Disease Node similarity features: DSS.csv
Metabolite similarity network: MPCS.csv
Disease similarity network: GIPD (Generated by the f5_pt.py file in the code)

# Model options
```
--hops                   int         Hop of neighbors to be calculated.         Default is 4.
--pe_dim                 int         position embedding size.                   Default is 256.
--n_layers               int         Number of Transformer layers.              Default is 1.
--n_heads                int         Number of Transformer heads.               Default is 8.
--hidden_dim             int         Hidden layer size.                         Default is 512.
--ffn_dim                int         FFN layer size.                            Default is 64.
--epochs                 int         Number of epochs to train.                 Default is 1000.
--dropout                float       Dropout.                                   Default is 0.3.
--attention_dropout      float       Dropout in the attention layer.            Default is 0.3.
```

# How to run?
```
1. f5_pt.py        # run f5_pt.py to generate the data needed for five-fold cross validation
2. main.py         # Run main.py to start the model
```
