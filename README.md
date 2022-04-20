# CycleGAN-with-Monet-Paintings
Capturing the special characteristics of Monet paintings inorder to turn ordinary pictures into Monet paintings

In a CycleGAN model we can obtain image-to-image translations without paired examples. This means the algorithm learns the specific features of an image that it then reproduces in the form of another image that has some similar features than the original one. This could mean for example learning the details of a zebra and transforming the images of horses into zebras, transforming a winter seasonal landscape into the same landscape but during summertime, or learning the specific stroke techniques and colors of a painter and transforming ordianry pictures into paintings.

The Generative Adversarial Network (GAN) trains two models at the same time: one that generates the sample and the other that discrminates the generated samples. In the CycleGAN two generators and two discriminators operate in a cycle that aim in making a replicate of the original picture that is as close as possible to the original. Each training update the generator becomes a bit better at making a replicate and the discriminator in turn, better at spotting a fake from the original. This eventually leads to a fast learning of the representations of the features that can be used not only in image-to-image translations but also in the creation of videos or music for example.

In this project I will implement a CycleGAN model that aims to refabricate the french painter Claude Monet's paintings from landscape pictures.
