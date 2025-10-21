In this folder, the artificial datasets, that were generated as part of our study (see https://doi.org/10.1016/j.jenvp.2025.102803 for further details) are listed. We trained [StyleGAN2-ADA](https://github.com/NVlabs/stylegan2-ada-pytorch) on the CalHouses dataset individually for each of our rating dimensions (hominess, invitingness, relaxation, safety, perceived price) and additionally also on the actual price of the houses. 

Each dimensions was split into four class ceatgories, representing the dimensions as shown in the Table below.
| Dimension | Class 0 | Class 1 | Class 2 | Class 3 |
|--------------|-----------|------------|-------|--------|
| **Hominess** | not homey | rather not homey | rather homey | homey |
| **Invitingness** | not inviting | rather not inviting | rather inviting | inviting |
| **Relaxation** | not relaxing | rather not relaxing | rather relaxing | relaxing |
| **Safety** | not safe | rather not safe | rather safe | safe |
| **Price** | cheap | rather cheap | rather expensive | expensive |

We generated a dataset for each dimension, with 500 images per class category, resulting in 2000 images per dataset. The class category an image is supposed to represent (as determined by the GAN) is shown in the file name. A file from the dataset of hominess with class0 indicates that this file is supposed to show a not homey house.