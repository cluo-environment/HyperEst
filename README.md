# HyperEst: Context-aware self-supervised pretraining for hyperspectral and multispectral water quality estimation (JAG 2025)

Chenxi Luo, Wei Xiang, Kang Han, Lu Yu, Yiqing Guo, S. L. Kesav Unnithan, Xiubin Qi, and Nagur Cherukuru

*La Trobe University and CSIRO*

## 📢 Latest Updates
- **5 August 2025**: Pretrained weights have been released and are now available for download.  
- **27 July 2025**: Our paper was accepted for publication in the **[International Journal of Applied Earth Observation and Geoinformation (JAG)](https://www.sciencedirect.com/journal/international-journal-of-applied-earth-observation-and-geoinformation)**.
---

## 🚀 Getting Started

### Prerequisites

Before proceeding with the installation, make sure the following dependencies are available on your system:

- **Conda 23.11.0** (Miniconda or Anaconda)  
  If you do not have Conda installed, download and install it from the [official Miniconda website](https://docs.conda.io/en/latest/miniconda.html).


### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/cluo-environment/HyperEst.git
    cd HyperEst
    ```
2.  **Create the Conda Environment:**
    ```bash
    conda env create -f environment.yml
    ```
3.  **Activate the environment:**
    ```bash
    conda activate HyperEst
    ```
### Dataset

1. **GLORIA:**
   * You can download the GLORIA dataset from [here](https://download.pangaea.de/dataset/948492/files/GLORIA-2022.zip)
2. **Lucinda Jetty**
   * You can download the Lucinda Rrs from [here](https://thredds.aodn.org.au/thredds/catalog/IMOS/SRS/OC/LJCO/catalog.html)
   * You can download the Lucinda water quality parameters from [here](https://thredds.aodn.org.au/thredds/catalog/IMOS/SRS/OC/BODBAW/catalog.html)

### Pretrained Weights

The following pretrained weights are available for use with this project:

| Model Name              | Description                                                                 | Download Link |
|-------------------------|-----------------------------------------------------------------------------|---------------|
| **HyperEst_1x1** | Pretrained model for the ablation study, utilizing only the **SPR** submodule. | [download](https://raw.githubusercontent.com/cluo-environment/HyperEst/refs/heads/main/pretrained/HyperEst_1x1.pth) |
| **HyperEst_5x5**         | Pretrained model incorporating both the **SPR** and **MSDL** submodules for full functionality. | [download](https://raw.githubusercontent.com/cluo-environment/HyperEst/refs/heads/main/pretrained/HyperEst_5x5.pth) |

## 🙌 Acknowledgements

We gratefully acknowledge the following open-source projects as benchmarks and baselines:  

* [MDN V2](https://github.com/ryan-edward-oshea/MDN_V2/tree/48d29db949bc8db6de41c1590d92836123c4ec2d)  
* [Hyper-VAE](https://github.com/CASELabCode/Jiadong-HyperVAE.git)  

We also thank the data providers for making the datasets publicly available:  

* GLORIA Dataset – provided by [PANGAEA Data Publisher](https://doi.org/10.1594/PANGAEA.948492).  
* Lucinda Jetty (IMOS) Datasets – provided by the [Integrated Marine Observing System (IMOS)](https://imos.org.au/), including:  
  * Remote sensing reflectance (Rrs) data  
  * Water quality parameter data  