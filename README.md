Dislocation-Loop-Analysis-through-Generative-AI-Leveraging-Variational-Autoencoders


![image](https://github.com/shradhautk/Dislocation-Loop-Analysis-through-Generative-AI-Leveraging-Variational-Autoencoders/assets/101154495/4bf31a19-cb7b-4a8c-9506-7cb3da3a64dd)


This code focuses on the training of Variational Autoencoders (VAEs) using image patches extracted from microscopy images containing irradiation induced dislocation loops to uncover latent representations. It introduces various types of VAEs, including:

Vanilla VAE: Featuring 2 continuous latent variables.
shVAE: A spatial VAE with translational invariance, utilizing 2 shift variables and 2 latent variables.
rVAE: A spatial VAE with rotational invariance, incorporating 1 rotation variable and 2 latent variables.
shrVAE: Combining translational and rotational invariance with 2 shift, 1 rotation, and 2 latent variables.
r_jvae: A joint VAE with rotational invariance and 3 discrete variables.
sh_jvae: A joint VAE with translational invariance and 5 discrete variables.
Key Highlights:

The code begins by loading a microscopy image, performing preprocessing, and generating a dataset from small image patches on a grid.
Custom PyTorch datasets and data loaders are defined to batch these image patches efficiently.
The initialization of various VAE types, encompassing both continuous and discrete latent variables.
Training these VAEs involves employing stochastic variational inference and visualizing the learned latent representations.
Encoding image patches into the latent space and spatially visualizing continuous and discrete latent variables.
Decoding samples from the latent space and assessing model performance through reconstruction error calculations.
Spatial and joint VAEs are designed to disentangle important factors of variation, such as location, rotation, and discrete features in the images.
The code leverages a custom PyroVED trainer to handle enumeration and SVI optimization during training.
In summary, this project trains VAEs to autonomously uncover meaningful representations within microscopy images. The inclusion of spatial and joint VAE architectures aims to disentangle essential latent factors within the dataset.





