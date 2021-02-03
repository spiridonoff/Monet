# Monet
The repo is made for the Kaggle competition "I’m Something of a Painter Myself" available here:
https://www.kaggle.com/c/gan-getting-started/data

Here, we train a GAN on Monet's paintings and use that to transform an input photo to one with the painting style of Monet. 

This project is inspired by paper https://arxiv.org/pdf/1703.10593.pdf Here, we try not to directly copy the codes of the repository provided for paper above, yet create a simplified CycleGan version of their work in a single notebook. However, some of the functions such as 'ResnetGenerator', 'ResnetBlock, 'GANloss' were used here since we didn't want to reinvent the wheel!

This notebook trains on two sets of photos, A: real photos of landscapes and B: paintings of Monet. The ultimate goal is to transform photos of each style to another (A -> B or B -> A). This is done by creating 2 generators and 2 discriminators. See paper above for more details.

This note book has the following main parts:

 - set up and define parameters
 - create datasets and dataloaders, visualize a batch of training data from sets A and B.
 - Define main CycleGAN model
 - Training Loop
 - Evaluate the trained model
