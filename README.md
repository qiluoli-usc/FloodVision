# FloodVision - DeepLabV3Plus for Flood Detection - Sen1Flood11

![Heade](img/Head.jpg)

## Synopsis

FloodVision leverages the power of Sentinel-2 satellite imagery and the [DeepLabV3+](https://arxiv.org/abs/2210.10732) deep learning architecture to detect and map flood-affected areas. This project utilizes Bands 11 (SWIR), 8 (NIR), and 4 (Red) from Sentinel-2 imagery to emphasize the spectral characteristics of water bodies and land cover changes, ensuring accurate segmentation of flood regions. By incorporating the [Sen1Floods11](https://github.com/cloudtostreet/Sen1Floods11)dataset, which provides labeled flood and non-flood regions, the project addresses the need for reliable and automated flood mapping solutions.

---

## About this Python Package

The repository contains two primary modules:

### Training Module  
Implements the DeepLabV3+ training pipeline using the `DeeplabV3Plus_RS_Train.ipynb` notebook with the following features:

   - Pre-trained weights: `deeplabv3_finetuned_RS_Sen1Flood11_V1.pth`,are not included in the GitHub repository due to their large size. You can download the file from the Google Drive: [Download Pre-trained Weights](https://drive.google.com/file/d/1a97fLOw_YLnb1PuQR7iny-X9O2DDRqLF/view?usp=sharing)
   - Configuration for semantic segmentation with 3 classes

### Inference Module
The `DeeplabV3Plus_RS_Predict.ipynb` notebook is used for batch processing of satellite images, generating flood predictions in .png format with color-coded classes.


---

## Acknowledgments

- **DeepLabV3+**: [https://arxiv.org/abs/2210.10732](https://arxiv.org/abs/2210.10732)
- **Sen1Floods11**: [https://github.com/cloudtostreet/Sen1Floods11](https://github.com/cloudtostreet/Sen1Floods11)

For questions or contributions, feel free to create issues or pull requests.
