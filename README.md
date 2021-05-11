Implementing DCGANs in Keras

Radford et al. (2015) Unsupervised representation learning with deep convolutional generative adverserial networks. (https://arxiv.org/abs/1511.06434)

- scale the range of the tanh activation function [-1,1]
- train models with mini-SGD (mini-batch size of 128)
- weights initialized from a zero-centered normal dist with stdev of 0.02
- use a leaky ReLU and the slope of the leak is set to .2 for all models
- use an Adam optimizer with tuned hyperparams. Leanring rate, alpha of .0002
- momentum term beta_1 at suggested val of .9 results in instability, so used .5
- in generator NN: use ReLU in all layers except for output which uses Tanh
- in discriminator NN: use Leaky ReLU in all layers
 
Data: https://www.kaggle.com/gasgallo/faces-data-new
<br> <br>
Output:
<br> <br>
Train 49
<br> 
![Train 49](https://raw.githubusercontent.com/kopalgarg/GAN-keras/main/output/train-49.png)
<br> <br>
Train 40
<br> 
![Train 40](https://raw.githubusercontent.com/kopalgarg/GAN-keras/main/output/train-40.png)
<br> <br>
Train 30 
<br> 
![Train 30](https://raw.githubusercontent.com/kopalgarg/GAN-keras/main/output/train-30.png)
<br> <br>
Train 20
<br> 
![Train 20](https://raw.githubusercontent.com/kopalgarg/GAN-keras/main/output/train-20.png)
<br> <br>
Train 10
<br> 
![Train 10](https://raw.githubusercontent.com/kopalgarg/GAN-keras/main/output/train-10.png)
<br> <br>
Train 1
<br> 
![Train 1](https://raw.githubusercontent.com/kopalgarg/GAN-keras/main/output/train-1.png)
