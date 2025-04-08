This study implemented a MolGAN architecture to generate novel molecules from a database of over 15,000 SMILES (Simplified Molecular Input Line Entry System) entries. The MolGAN architecture is trained adversarially via the Wasserstein GAN with Gradient Penalty (WGAN-GP) framework to generate realistic molecular graphs. A generator network maps latent vectors to graph tensors, while a Relational Graph Convolutional Network (RGCN)-based discriminator learns to approximate the Wasserstein distance between real and generated graph distributions, stabilized by the gradient penalty. 
The generated molecules were evaluated after training for several hundred epochs using established drug-likeness metrics and tanimoto analysis. The heatmap visualization demonstrated distinct clusters of molecular scaffolds, indicating the model's ability to explore various regions of chemical space. Analysis of drug-likeness metrics showed that a significant proportion of the generated molecules satisfied Lipinski's Rule of Five and exhibited favorable QED scores. However, the model is failing significantly to reproduce the aromatic character that appears dominant in the original database, suggesting a need for more rigorous training.
