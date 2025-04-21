# CDR-Net

Official PyTorch implementation of **CDR-Net: Collaborative Dual-network Region-based Distillation for Semi-Supervised Medical Image Segmentation**.

The full codebase will be publicly available upon the acceptance of our paper.

---

## 🔔 Note

Thank you for your interest in our work!  
As the paper is currently under review, we are only sharing the minimal setup to get model performance using pre-trained models.

You can still explore the performance of our method by using the models provided in the [release page](https://github.com/ridvan25/CDR-Net/releases/tag/release_1.0.0_cdrnet).

- `vnet_best.pth` is the pre-trained weight for the **VNet sub-network** trained with **region-based intra- and inter-network distillation**. 

- `resnet_best.pth` is the pre-trained weight for the **3D-ResVNet sub-network** trained jointly with VNet in our CDR-Net framework.

You can use these weights to:
- Perform direct inference using `test_LA_CDR-Net.py`
- Benchmark against your methods


## ✅ Inference Results

You can reproduce the following results by running the `test_LA_CDR-Net.py` script with the provided pre-trained weights:

`bash
python test_LA_CDR-Net.py` 

The script will output average performance metrics as shown below:

average metric is [0.91102777  0.83725662  5.10892647  1.5907378]

The script will output average performance metrics as shown below:

Dice Score | Jaccard Index | 95% Hausdorff Distance (95HD) | Average Surface Distance (ASD)

0.9110     |      0.8373   |            5.109              |              1.591

## 🙏 Acknowledgement

We build the project based on **MCF**, **UA-MT**, **SASSNet**, and **DTC**.  
Thanks to the authors of these works for their valuable contributions and open-source efforts.



