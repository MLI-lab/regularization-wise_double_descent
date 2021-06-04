# Regularization-wise double descent
This repository contains the code for reproducing figures and results in the paper ``Regularization-wise double descent: Why it occurs and how to eliminate it''.

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