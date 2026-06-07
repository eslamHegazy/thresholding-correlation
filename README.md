[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

# Image Thresholding: Understanding Bias of Evaluation Metrics Towards Specific Evaluation Functions

Official implementation accompanying the paper:

**Eslam Hegazy, Mohamed Gabr**
*Image Thresholding: Understanding Bias of Evaluation Metrics Towards Specific Evaluation Functions*
Accepted at **ICPR 2026** and to appear in the conference proceedings.

**Preprint (earlier draft version):**
https://arxiv.org/abs/2605.27132

> **Note:** The arXiv manuscript corresponds to a preprint submitted prior to publication. Minor revisions may exist between the preprint and the final version that will appear in the ICPR 2026 proceedings.

## Overview

This repository contains the code used to analyze the relationship between image thresholding objective functions and commonly used evaluation metrics. The study investigates the extent to which evaluation metrics exhibit bias toward specific thresholding objective functions, particularly Otsu's between-class variance and Kapur's entropy. Experiments are conducted on the BSDS500 dataset.

## Repository Structure

```text
.
├── analysis.ipynb
├── requirements.txt
├── BSDS500-master/
├── LICENSE
└── README.md
```

* `analysis.ipynb` contains the complete experimental workflow and reproduces the results presented in the paper.
* `requirements.txt` lists the required Python packages.
* `BSDS500-master/` contains the BSDS500 dataset.

## Installation

Install the required dependencies:

```bash
pip install -r requirements.txt
```

The code was tested with **Python 3.9**.

## Dataset

Only a small subset of BSDS500 images is included in this repository for demonstration purposes.

To reproduce the results reported in the paper, the complete BSDS500 dataset is required.

### Downloading BSDS500

Download the dataset from the GitHub mirror:

* Repository: https://github.com/BIDS/BSDS500
* ZIP archive: https://github.com/BIDS/BSDS500/archive/refs/heads/master.zip

After downloading and extracting the archive, place the extracted folder in the repository root so that the structure becomes:

```text
.
├── analysis.ipynb
├── requirements.txt
├── README.md
└── BSDS500-master/
    └── BSDS500/
        └── data/
            ├── images/
            │   ├── train/
            │   ├── val/
            │   └── test/
            └── groundTruth/
                ├── train/
                ├── val/
                └── test/
```

## Reproducing the Results

1. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Download and extract the BSDS500 dataset as described above.

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open `analysis.ipynb`.

5. Execute all notebook cells from top to bottom.

## Citation

If you use this code in your research, please cite:

```bibtex
@misc{hegazy2026imagethresholdingunderstandingbias,
      title={Image Thresholding: Understanding Bias of Evaluation Metrics towards Specific Evaluation Functions}, 
      author={Eslam Hegazy and Mohamed Gabr},
      year={2026},
      eprint={2605.27132},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2605.27132}, 
}
```

The currently available arXiv version is a preprint. Once the official ICPR proceedings version becomes available, the citation information will be updated accordingly.


## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
