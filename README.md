# Regularization-wise double descent
This repository contains the code for reproducing figures and results in the paper ``Regularization-wise double descent: Why it occurs and how to eliminate it''.

**Note:** Proof of theoretical results and additional numerical experiments are provided [here](appendix.pdf).

# Requirements
The following Python libraries are required to run the code in this repository:

```
numpy
jupyter
torch
torchvision
```
and can be installed with `pip install -r requirements.txt`.

# Usage
The figures in the paper can be reproduced by running the respective notebooks as indicated below:

**Figure 1**: Regularization-wise double descent for the 5-layer CNN trained on CIFAR-10 with 20% label noise can be reproduced by running the `regularization-wise_deep_double_descent` notebook.

**Figure 2**: Bias-variance trade-off curves for the linear ridge regression can be reproduced by running the `sum_bias_variance_tradeoffs` notebook.

**Figure 3, 4**: Regularization-wise double descent for the two layer neural network and the norm of the change in the parameters of the two layer network relevant and non-relevant to fitting the data can be reproduced by running the `two-layer-nn_regularization-wise_double_descent` notebook. 

The numerical results can be reproduced by training the models with `python3 train_<SETTING>.py --config $CONFIG_FILE` where `CONFIG_FILE` points to the `config.json` file of the desired setup in the `./results/` directory.

## Citation
```
@inproceedings{yilmaz_heckel_2022,
    author    = {Fatih Furkan Yilmaz and Reinhard Heckel},
    title     = {Regularization-wise double descent: Why it occurs and how to eliminate it},
    booktitle = {IEEE International Symposium on Information Theory (ISIT)}
    year      = {2022}
}
```

## Licence

All files are provided under the terms of the Apache License, Version 2.0.