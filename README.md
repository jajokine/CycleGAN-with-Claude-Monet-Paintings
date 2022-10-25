<h1 align='center'>CycleGAN with Claude Monet Paintings</h1>

<p align='center'>
      <img
           width='1000'
           height='400'
           src='https://github.com/jajokine/CycleGAN-with-Monet-Paintings/blob/main/Images/banner.png'
      >
</p>

In a CycleGAN model we can obtain image-to-image translations without paired examples. This means the algorithm learns the specific features of an image that it then reproduces in the form of another image that has similar features compared to the original one. In fact, so similar that it is difficult to spot a generated image from the original one. This could mean for example learning the details of a zebra and transforming the images of horses into zebras. Or we could have a winter seasonal landscape transformed into the same landscape but during summertime.

In this project we will try to learn the specific brush stroke techniques and color-usage of the French painter Claude Monet and transform ordinary pictures into paintings. I will follow a similar model that was introduced in the CycleGAN research paper, but with a different kind of generator that two competing objectives push to excel in generating the images (Jun-Yan Zhu, Taesung Park, Phillip Isola and Alexei A. Efros, (2020), "Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks", arXiv:1703.10593). 

The CycleGAN model has a similar structure than a Generative Adversarial Network (GAN) that trains two models at the same time: one that generates a replicate of an original sample and the other that discriminates the generated replicates. However, in the CycleGAN we have two generators and two discriminators that operate in a cycle aimed in making a replicate of the original picture that is as close as possible to the original. This is the same as training a model to translate a sentence from English to French, and then translating this sentence again back from French to English, but with image instead of the sentences.  Each training update the generators become a bit better at making replicates, and the discriminators in turn, better at spotting a fake from the original. One generator focuses on transforming a picture into a painting and the other transforming a painting into a picture. The two discriminators then try to spot the mistakes made in the replicates, and eventually learn the feature representations of the paintings. It will be interesting to see how well a computer-based model is able to perform in this kind of tasks which usually demand creativity and vision that try to capture feelings and emotions.  


