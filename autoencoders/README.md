# Auto Encoders Variational and Otherwise

Some experiements with autoencoders as dimensionality reduction and as learning manifolds from data.
This includes the original paper and a little notebook flushing out the reparameterization trick which is the heart of VAEs.

One experiment is having a high dimensional vector which only has 2 values placed in random indices. 
Interestingly the vanilla autoencoder trivially learns this task but the training is very difficult
with the VAE. The original paper would dictate having the loss be the neg log likelihood but else where 
people use MSE and this seems to in fact work better. I could never get the network to learn using the full
loss that the theory would suggest. 

For MNIST however the VAE does quite well (even with a 2 dimensional latent space!) as evidenced by the manifold of the latent space at the end.
