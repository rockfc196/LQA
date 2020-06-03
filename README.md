# LQA

In deep learning tasks, the learning rate determines the update step size in each iteration, which plays a critical role in gradient-based optimization. However, the determination of the appropriate learning rate in practice typically replies on subjective judgement. In this work, we propose a novel optimization method based on local quadratic approximation (LQA). In each update step, given the gradient direction, we locally approximate the loss function by a standard quadratic function of the learning rate. Then, we propose an approximation step to obtain a nearly optimal learning rate in a computationally efficient way. The proposed LQA method has three important features. First, the learning rate is automatically determined in each update step. Second, it is dynamically adjusted according to the current loss function value and the parameter estimates. Third, with the gradient direction fixed, the proposed method leads to nearly the greatest reduction in terms of the loss function. Extensive experiments have been conducted to prove the strengths of the proposed LQA method. The detailed description of the LQA method can be found at https://arxiv.org/abs/2004.03260.

To support real applications involving the training of neural networks, we have developed an implementation of the LQA method based on PyTorch. This implementation can provide an alternative method for users to accelerate the training of their models. To use this implementation, please import the file `LQA.py` and call the LQA method in the update step. The Jupyter file `demo.ipynb` gives an example for how to use it in the training of a LetNet model.
