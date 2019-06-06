## Paper

_Wen-Chin Huang, Hao Luo, Hsin-Te Hwang, Chen-Chou Lo, Yu-Huai Peng, Yu Tsao, Hsin-Min Wang,_ **Unsupervised Representation Disentanglement using Cross Domain Features and Adversarial Learning in Variational Autoencnder based Voice Conversion**, June 2019

## CDVAE-GAN-CLS-VC

![methods](/imgs/entangled-vc.png)

An effective approach for voice conversion (VC) is to disentangle linguistic content from other components in the speech signal. The effectiveness of variational autoencoder (VAE) based VC (VAE-VC), for instance, strongly relies on this principle. In our [prior work](https://unilight.github.io/CDVAE-Demo/), we proposed a cross-domain VAE-VC (CDVAE-VC) framework, which utilized acoustic features of different properties, to improve the performance of VAE-VC. We believed that the success came from more disentangled latent representations. In this paper, we extend the CDVAE-VC framework by incorporating the concept of adversarial learning, in order to further increase the degree of disentanglement, thereby improving the quality and similarity of converted speech. More specifically, we first investigate the effectiveness of incorporating the generative adversarial nets (GANs) with CDVAE-VC. Then, we consider the concept of domain adversarial training and add an explicit constraint to the latent representation, realized by a speaker classifier, to explicitly eliminate the speaker information that resides in the latent code. Experimental results confirm that the degree of disentanglement of the learned latent representation can be enhanced by both GANs and the speaker classifier. Meanwhile, subjective evaluation results in terms of quality and similarity scores demonstrate the effectiveness of our proposed methods.

## Subjective Evaluation Results

We evaluated our proposed framework on the **Voice Conversion Challenge 2018 (VCC 2018) dataset**. [[Paper]](https://arxiv.org/abs/1804.04262)[[Dataset]](https://datashare.is.ed.ac.uk/handle/10283/3061)


### MOS on naturalness

![Naturalness](/imgs/mos.png)

### Conversion accuracy

![Similarity](/imgs/similarity.png)

## Speech Samples

### SF1-TF1

|Type|Sample|
|:--|:--|
|Source|<audio controls="controls"><source type="audio/wav" src="samples/natural/SF1-30001.wav"></source></audio>|
|Target|<audio controls="controls"><source type="audio/wav" src="samples/natural/TF1-30001.wav"></source></audio>|
|CDVAE+GV|<audio controls="controls"><source type="audio/wav" src="samples/cdvae/SF1-TF1-30001-gv.wav"></source></audio>|
|CDVAE-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-gan/SF1-TF1-30001.wav"></source></audio>|
|CDVAE-CLS-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-cls-gan/SF1-TF1-30001.wav"></source></audio>|

### SF1-TM1

|Type|Sample|
|:--|:--|
|Source|<audio controls="controls"><source type="audio/wav" src="samples/natural/SF1-30001.wav"></source></audio>|
|Target|<audio controls="controls"><source type="audio/wav" src="samples/natural/TM1-30001.wav"></source></audio>|
|CDVAE+GV|<audio controls="controls"><source type="audio/wav" src="samples/cdvae/SF1-TM1-30001-gv.wav"></source></audio>|
|CDVAE-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-gan/SF1-TM1-30001.wav"></source></audio>|
|CDVAE-CLS-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-cls-gan/SF1-TM1-30001.wav"></source></audio>|

### SM1-TF1

|Type|Sample|
|:--|:--|
|Source|<audio controls="controls"><source type="audio/wav" src="samples/natural/SM1-30001.wav"></source></audio>|
|Target|<audio controls="controls"><source type="audio/wav" src="samples/natural/TF1-30001.wav"></source></audio>|
|CDVAE+GV|<audio controls="controls"><source type="audio/wav" src="samples/cdvae/SM1-TF1-30001-gv.wav"></source></audio>|
|CDVAE-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-gan/SM1-TF1-30001.wav"></source></audio>|
|CDVAE-CLS-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-cls-gan/SM1-TF1-30001.wav"></source></audio>|

### SM1-TM1

|Type|Sample|
|:--|:--|
|Source|<audio controls="controls"><source type="audio/wav" src="samples/natural/Sm1-30001.wav"></source></audio>|
|Target|<audio controls="controls"><source type="audio/wav" src="samples/natural/TM1-30001.wav"></source></audio>|
|CDVAE+GV|<audio controls="controls"><source type="audio/wav" src="samples/cdvae/SM1-TM1-30001-gv.wav"></source></audio>|
|CDVAE-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-gan/SM1-TM1-30001.wav"></source></audio>|
|CDVAE-CLS-GAN-MCC|<audio controls="controls"><source type="audio/wav" src="samples/cdvae-cls-gan/SM1-TM1-30001.wav"></source></audio>|