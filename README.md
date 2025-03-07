# RLEM
Note: Read the details of the project are given below. The code is currently under scrutiny for open-source at LANL.
### Reverse latent evolution model (RLEM) for time-inversion of spatiotemporal dynamics
##### 
- It combines a conditional variational autoencoder (CVAE) to project high-dimensional data into a lower-dimensional latent distribution. Subsequently, a LSTM network learns the reverse temporal dynamics within this latent space. During the prediction stage, both networks are integrated into an autoregressive loop to estimate all the upstream fields given limited downstream measurements.

<p align="center">
  <img src="images/model.png" width="450" height="260" />
</p>

- VAE's latent space encodes the aleatoric uncertainty of the higher-dimensional input dataset. This uncertainity can be propgated through the temporal learner to predict upstream fields with uncertainty bounds.

- This repository contains codes accompanying the [paper](https://arxiv.org/abs/2408.07847). The dataset accompying the paper is available at Zenodo.  <a href="https://doi.org/10.5281/zenodo.10819001"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.10819001.svg" alt="DOI"></a>
