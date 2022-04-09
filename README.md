# Test Pytorch / TensorFlow on M1
Super simple Code and resources to test training a CNN on M1 macbook.

## Install PyTorch and TensorFlow for M1
- PyTorch: see this [blog](https://towardsdatascience.com/yes-you-can-run-pytorch-natively-on-m1-macbooks-and-heres-how-35d2eaa07a83).
- TensorFlow: see this [blog](https://makeoptim.com/en/deep-learning/tensorflow-metal).

## Run tests using PyTorch and TensorFlow
### 1. PyTorch
Run `mnist_cnn_pt.py` on M1 CPU (GPU not supported yet). Finished in ~6 mins. Results are shown below.
```
Test set: Average loss: 0.0254, Accuracy: 9919/10000 (99%)
python mnist_cnn.py  903.89s user 331.90s system 306% cpu 6:43.59 total
```

### 2. TensorFlow
Run `mnist_cnn_tf.py` on M1 GPU natively. Finished in ~1 min. Results are shown below.
```
Test Accuracy: 0.9909000396728516
python mnist_cnn_tf.py  43.96s user 18.72s system 64% cpu 1:37.17 total
```

## My Macbook Spec
- OS: macOS 12.2.1
- Model: MacBook Pro (16-inch, 2021)
- Chip: Apple M1 Pro
- RAM: 32 GB

## More comprehensive evaluations
- Please see [this blog](https://wandb.ai/tcapelle/apple_m1_pro/reports/Deep-Learning-on-the-M1-Pro-with-Apple-Silicon---VmlldzoxMjQ0NjY3).
