## Artificial Datasets

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

Please note that each dataset folder contains folders "part1" and "part2". This is due to the fact that github omitts files, if a folder contains more than 1000 files. The dataset is only complete if "part1" and "part2" are considered together.

Each dataset folder further holds a csv file with participants' ratings on the artificial datasets, which were collected in an online study. Each image was rated on a 0-100 visual analogue scale by 10-12 participants. The provided rating is an average across all responses. Please view our article for more information about the online study.

## Model Weights

The model weights for each dimensions can be downloaded here:

* [Hominess](https://drive.google.com/file/d/1CSUfH5PLMeoLzGmtAiWLvYbtug-OLYbm/view?usp=sharing)
* [Invitingness](https://drive.google.com/file/d/1Jj5GVNHkMtQisJIwTz4zQ3Bx2tkIe9qR/view?usp=sharing)
* [Relaxation](https://drive.google.com/file/d/1Vf0VSk1GsmJp7xmrRtnumwvvXjbjFmT9/view?usp=sharing)
* [Safety](https://drive.google.com/file/d/1QigHGnc6Ecd1fe0ILYXx87VqdvXYIDXn/view?usp=sharing)
* [Perceived price](https://drive.google.com/file/d/1yExyuNnYmsi0Wu2ngFyz3HfumKmPOiSo/view?usp=sharing)
* [Actual price](https://drive.google.com/file/d/1O_wIKuNNj_qPtHQB6SI-IlLHoZwfXAuD/view?usp=sharing)