# Data-Driven Method for Li-Ion Battery Health Monitoring

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.7.0-orange.svg)](https://pytorch.org/)

## Table of Contents

- [Description](#description)
- [Key Features](#key-features)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Download the Dataset](#download-the-dataset)
  - [Setup](#setup)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Contributing](#contributing)
- [Credits](#credits)
- [Acknowledgement](#acknowledgement)
- [Star History](#star-history)

## Description 

Li-Ion batteries are increasingly being used due to sustainable development goals and the numerous benefits they provide compared to other battery technologies. Accurate prediction of State-of-Health (SOH) for Li-Ion batteries has become critically important, and data-driven online SOH prediction models offer an efficient approach to address this challenge.

**We propose a simple yet effective machine learning framework utilizing Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU) models for SOH prediction, addressing the common issues of high complexity, low interpretability, and high training costs. Our GRU-based predictions demonstrate high accuracy with an average Root Mean Squared Error (RMSE) of 0.724%.**

## Key Features

- 🔋 **Battery Health Monitoring**: Advanced SOH prediction for Li-Ion batteries
- 🧠 **Deep Learning Models**: Implementation of LSTM and GRU architectures
- 📊 **High Accuracy**: Achieves 0.724% RMSE with GRU model
- 📈 **Data-Driven Approach**: Utilizes real battery degradation data
- 🚀 **Easy to Use**: Simple setup and execution with Jupyter notebooks
- 📚 **Well Documented**: Comprehensive documentation and examples

## Prerequisites

Before you begin, ensure you have the following installed:

- **Python 3.10** or higher
- **Jupyter Notebook** or **JupyterLab**
- **Git** (for cloning the repository)
- At least **4GB RAM** (recommended for dataset processing)
- **500MB disk space** for dataset and dependencies

## Getting Started

### Download the Dataset

This project uses the open source [Oxford Battery Degradation Dataset 1](https://ora.ox.ac.uk/objects/uuid:03ba4b01-cfed-46d3-9b1a-7d4a7bdf6fac) [1].

> **Important**: These data are copyright (c) 2017, The Chancellor, Masters and Scholars of the University of Oxford, and the 'Oxford Battery Degradation Dataset 1' researchers. All rights reserved.

> The dataset is made available under the [Open Database License](http://opendatacommons.org/licenses/odbl/1.0/) with individual contents licensed under the [Database Contents License](http://opendatacommons.org/licenses/dbcl/1.0/).

**Steps to download:**

1. Visit the [dataset download page](https://ora.ox.ac.uk/objects/uuid:03ba4b01-cfed-46d3-9b1a-7d4a7bdf6fac/files/m5ac36a1e2073852e4f1f7dee647909a7)
2. Download the file `Oxford_Battery_Degradation_Dataset_1.mat` (⚠️ **262MB file**)
3. Place the downloaded file in the `./datasets/` directory

📝 **Note**: The [dataset readme file](https://github.com/sileneer/NRP_2022_EEE12/blob/main/datasets/Readme.txt) contains detailed information about the data structure and format.

### Setup

Follow these steps to set up your development environment:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sileneer/NRP_2022_EEE12.git
   cd NRP_2022_EEE12
   ```

2. **Create a virtual environment:**
   ```bash
   python3.10 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

## Usage

Once you have completed the setup and downloaded the dataset:

1. **Open the main notebook:**
   - Launch Jupyter Notebook: `jupyter notebook`
   - Open `main_torch.ipynb`

2. **Run the analysis:**
   - Execute cells sequentially to load data, train models, and generate predictions
   - The notebook includes both LSTM and GRU model implementations
   - Results and visualizations will be generated inline

3. **Model Training:**
   - The notebook automatically loads the Oxford dataset
   - Preprocessing steps include data normalization and sequence preparation
   - Both LSTM and GRU models are trained and compared

## Project Structure

```
NRP_2022_EEE12/
├── datasets/                    # Dataset directory
│   ├── Readme.txt              # Dataset documentation
│   └── Oxford_Battery_...mat   # Main dataset (download required)
├── literature_reviews/         # Research papers and references
├── saved_models/              # Trained model checkpoints
├── main_torch.ipynb          # Main analysis notebook
├── requirements.txt          # Python dependencies
├── README.md                # This file
└── LICENCE                  # MIT License
```

## Results

Our machine learning framework demonstrates excellent performance in predicting Li-Ion battery State-of-Health:

- **GRU Model Performance**: 
  - Average RMSE: **0.724%**
  - High accuracy in SOH prediction
  - Efficient training time
  
- **LSTM Model Performance**:
  - Competitive accuracy
  - Good generalization across different battery cells

The models successfully address common challenges in battery health monitoring:
- ✅ **Low Complexity**: Simple architecture easy to understand and implement
- ✅ **High Interpretability**: Clear model behavior and prediction rationale  
- ✅ **Low Training Cost**: Efficient training process with minimal computational requirements

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

**How to contribute:**

1. **Fork the Project**
2. **Create your Feature Branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your Changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the Branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

## Credits

This project uses the following open source libraries and frameworks:

- **[PyTorch](https://pytorch.org/)** - Deep learning framework for model implementation
- **[NumPy](https://numpy.org/)** - Numerical computing library
- **[Pandas](https://pandas.pydata.org/)** - Data manipulation and analysis
- **[Matplotlib](https://matplotlib.org/)** - Plotting and visualization
- **[Scikit-learn](https://scikit-learn.org/)** - Machine learning utilities
- **[SciPy](https://scipy.org/)** - Scientific computing library

## Acknowledgement 

This project is licensed under the [MIT License](https://github.com/sileneer/NRP_2022_EEE12/blob/main/LICENCE).

We extend our sincere appreciation to **David Howey** and **Christoph Birkl** for their invaluable work in collecting the `Oxford_Battery_Degradation_Dataset_1` and their ongoing research contributions. Their work can be found at: https://scholar.google.co.uk/citations?hl=en&user=AZdBXIkAAAAJ&view_op=list_works&sortby=pubdate

### References

[1] Christoph R. Birkl, "Diagnosis and Prognosis of Degradation in Lithium-Ion Batteries", PhD thesis, Department of Engineering Science, University of Oxford, 2017.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=sileneer/NRP_2022_EEE12&type=Date)](https://star-history.com/#sileneer/NRP_2022_EEE12&Date) 
