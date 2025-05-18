# Enhancing Ottoman Word Recognition via Self-Supervised Pretraining Using a Siamese Swin Transformer

This repository contains the code and resources for our research paper on semi-supervised Ottoman word recognition from historical handwritten documents, presented at IEEE SIU. Our method utilizes a two-stage approach: self-supervised pretraining followed by supervised training with triplet loss, employing a Siamese network architecture with a Shifted Window Transformer backbone. We demonstrate that pretraining significantly enhances the model's ability to discriminate between similar Ottoman words.

## Authors

* Sadiq Qara ([sadig.gara@sabanciuniv.edu](mailto:sadig.gara@sabanciuniv.edu), Sabanci University)<sup>\*</sup>
* Kourosh Sharifi ([kourosh.sharifi@sabanciuniv.edu](mailto:kourosh.sharifi@sabanciuniv.edu), Sabanci University)<sup>\*</sup>
* Mehmet Kuru ([mehmet.kuru@sabanciuniv.edu](mailto:mehmet.kuru@sabanciuniv.edu), Sabanci University)
* Sultan Toprak ([stoprakoker@unr.edu](mailto:stoprakoker@unr.edu), University of Nevada)
* Erchan Aptoula ([erchan.aptoula@sabanciuniv.edu](mailto:erchan.aptoula@sabanciuniv.edu), Sabanci University)

<sup>\*</sup>Equal Contribution

## Repository Structure

The repository is organized as follows:

* `notebooks/`: This directory will contain the Jupyter notebooks detailing the code implementation.
    * `PDF_to_Image_to_Processing.ipynb`: For applying preprocessing on the input file (PDF) to extract the necessary outputs (connected components, line segmentations, etc.).
    * `...` (add other notebook names and descriptions)
* `dataset/`: This directory will contain a README file pointing to the Google Drive folder containing the dataset.
* `requirements.txt`: A list of Python libraries necessary to run the code.

**Dataset:**

The dataset used in this research is available on Google Drive at [this link](https://drive.google.com/drive/folders/1jVk7BRCfLWznctXWx5WJRaJHWXSBymRB?usp=drive_link). It contains the following subfolders:

* `PDF-TO-JPEG/`: This folder contains the preprocessed image crops generated from PDF documents.
* `padded-KWS-Crops/`: This folder contains the labeled and padded keyword crops used for training and evaluation.

## Setup and Installation

To run the notebooks, you will need to set up a Python virtual environment and install the required libraries. You can do this using the following steps:

1.  **Create a virtual environment (optional but recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Linux/macOS
    # venv\Scripts\activate  # On Windows
    ```

2.  **Install the required libraries:**
    You can install all the necessary libraries using the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```
    Alternatively, you can install the libraries directly within a Jupyter notebook cell using the following:
    ```python
    !pip install -r requirements.txt
    ```

---

# Citation

If you use this code or dataset in your research, please cite our paper as follows:

```bibtex
@inproceedings{979-8-3315-6655-5,
  author={Sadiq Qara and Kourosh Sharifi and Mehmet Kuru and Sultan Toprak and Erchan Aptoula},
  booktitle={Proceedings of the [Year] IEEE Signal Processing and Communications Applications Conference (SIU)},
  title={Enhancing Ottoman Word Recognition via Self-Supervised Pretraining Using a Siamese Swin Transformer},
  year={2025},
  doi={Paper DOI (when available)}
  note={979-8-3315-6655-5/25/$31.00 ©2025 IEEE}
}
```

---

# Copyright

© 2025 IEEE. Personal use of this material is permitted. Permission from IEEE must be obtained for all other uses, in any current or future media, including reprinting/republishing this material for advertising or promotional purposes, creating new collective works, for resale or redistribution to servers or lists, or reuse of any copyrighted component of this work in other works.
