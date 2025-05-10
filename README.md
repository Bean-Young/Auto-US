# Auto-US

This project was created by [***Yuezhe Yang***](https://bean-young.github.io) for the paper **"Auto-US: An Ultrasound Video Diagnosis Agent Using Video Classification Framework and LLMs"** [Paper Link](http://exemple.com).

### Abstract

AI-assisted ultrasound video diagnosis offers new opportunities for improving the efficiency and accuracy of medical ultrasound imaging analysis. However, existing research has shortcomings in both dataset construction, accuracy, and clinical feasibility. In this study, we have proposed an ultrasound video diagnosis agent, **Auto-US**. First, we constructed a comprehensive ultrasound video dataset by integrating multiple open-access data sources. Then, we designed a novel CNN-Transformer network that fully leverages spatial, temporal, and frequency-domain information in ultrasound videos, achieving an accuracy of 86.73%. Finally, by integrating large language models, we conducted tests on clinical cases, demonstrating the potential of our model in practical applications. Our work highlights the potential of AI in ultrasound diagnosis and provides a valuable reference for future research in this field.

### Prepare Data

We constructed a **comprehensive dataset** that integrates multiple existing open access data sources, covering five typical disease categories and three different body parts.

The details of the datasets used and their specific links are provided here for easy access to the data.

#### BUV Dataset

The BUV (Breast Ultrasound Video) Dataset is a collection of ultrasound videos specifically designed for **breast lesion detection**. It is used to train and evaluate models for identifying and classifying breast lesions in ultrasound videos.

We used this dataset to train and evaluate our model for breast lesion detection, focusing on distinguishing between **benign and malignant lesions**.

[Download Link](https://github.com/jhl-Det/CVA-Net)

#### UIdataGB

The UIdataGB dataset is an ultrasound image dataset focused on **gallbladder diseases**, encompassing nine distinct categories of gallbladder diseases, with each category representing a specific type of gallbladder disease.

**In our study, we consolidated the nine different categories into one unified label for gallbladder diseases.**

[Download Link](https://data.mendeley.com/datasets/r6h24d2d3y/1)

#### POCUS

The POCUS dataset (Point-of-Care Ultrasound dataset) is a collection of **lung ultrasound images and videos** assembled from publicly available resources and publications. It is primarily designed for the detection and classification of lung diseases, particularly COVID-19 and bacterial pneumonia.

In our study, we utilized **33 videos of COVID-19 and 36 videos of bacterial pneumonia from the POCUS dataset, without distinguishing between Convex and Linear probe types**.

[Download Link](https://github.com/cossiomanuel/covid19_pocus_ultrasound/tree/master/data)

#### Butterfly

The Butterfly dataset is part of the US-4 dataset, which is included in the repository for [USCL](https://github.com/983632847/USCL) (Ultrasound Semi-Supervised Contrastive Learning).

To enhance the generalization capability of our model, we **integrated 20 videos of COVID-19 pneumonia from the Butterfly dataset** with the COVID-19 pneumonia videos from the POCUS dataset, treating them as a unified label.

[Download Link](https://github.com/983632847/USCL)

**In summary, the composition of the comprehensive dataset we constructed is shown in the table below:**

| Dataset     | Class                             | Sample   |
| :---------- | :-------------------------------- | :------- |
| BUV Dataset | Benign / Malignant Breast Lesions | 74 / 112 |
| UIdataGB    | Gallbladder Disease               | 220      |
| POCUS       | COVID-19 / Bacterial Pneumonia    | 33 / 36  |
| Butterfly   | COVID-19 Pneumonia                | 20       |

### Data Preprocessing

bala，npy……

### Usage

#### Installation

##### requirements

- Pytorch 2.0 (CUDA 11.8)
- For details on the environment, please refer to the requirements.txt file.

#### Training

#### Inference

### Results

### Bibtex

If you use this code or found it helpful, please consider citing:

```
@example{

}

```
