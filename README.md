# Galaxy Morphology Classification with Convolutional Neural Networks

This repository contains an end-to-end pipeline for **galaxy morphology classification** using **Deep Learning** and **Convolutional Neural Networks (CNNs)**.  
The goal is to automatically classify galaxies into the main classes of the **Hubble Sequence**, divided into two different schemes:

- Simple: E, S, SB  
- Classic: E0, E3, E7, S0, Sa, Sb, Sc, SBa, SBb, SBc  

The models use **transfer learning** with architectures such as **ResNet50** and **EfficientNet**, adapted for astronomical imaging tasks.

---

## Project Overview

Modern sky surveys like the **SDSS** produce millions of galaxy images, making manual classification increasingly impractical.  
This project builds an automated system that recognizes visual features present in RGB images of galaxies, such as spiral arms, disks, bulges, and bars, in order to classify each galaxy into its corresponding Hubble sequence class.

The dataset used is **Galaxy Zoo 2**, which provides volunteer-generated morphological labels. Since the original categories do not follow the classical Hubble sequence, this project implements a **mapping step** to convert Galaxy Zoo 2 labels into standardized Hubble classes, ensuring consistency across all processed datasets. Furthermore, all required data is automatically downloaded by the provided scripts.

The system applies **preprocessing**, **data augmentation**, and **hyperparameter tuning**, and evaluates performance using common metrics such as accuracy, F1-score, and confusion matrices.

---

## Author

**Gabriel Rocha Pinto**

## License

This project is licensed under the MIT License, see [LICENSE.txt](LICENSE.txt) for more information.
