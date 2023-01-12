# Data-Driven Method for Li-Ion Battery Health Monitoring

This project is under Nanyang Research Programme (NRP) by Nanyang Technological University (NTU), Singapore. The project code is EEE12 (2022). 

## Description 

> Li-Ion batteries are increasing in usage due to the aim of sustainable development and other benefits it provides as compared to other batteries. Being able to predict the SOH of Li-Ion Batteries has also grown in importance, and the method of data-driven model online state-of-health (SOH) prediction is an efficient way of completing the task necessary. **We proposed a simple and effective ML framework with long short-term memory (LSTM) and Gated Recurrent Unit (GRU) model for this situation to predict SOH, avoiding the problems of high complexity, low interpretability, and high training costs. Predictions made using GRU have shown to be of high accuracy with an average root mean squared error (RMSE) of 0.724%.**
 
## Getting Start

### Download the dataset

This project use the open source dataset [Oxford Battery Degradation Dataset 1](https://ora.ox.ac.uk/objects/uuid:03ba4b01-cfed-46d3-9b1a-7d4a7bdf6fac) [1]. 

> These data are copyright (c) 2017, The Chancellor, Masters and Scholars of the University of Oxford, and the 'Oxford Battery Degradation Dataset 1' researchers. All rights reserved.

> This 'Oxford Battery Degradation Dataset 1' is made available under the Open Database License: http://opendatacommons.org/licenses/odbl/1.0/. Any rights in individual contents of the database are licensed under the Database Contents License: http://opendatacommons.org/licenses/dbcl/1.0/

The [Readme](https://github.com/sileneer/NRP_2022_EEE12/blob/main/datasets/Readme.txt) file for the dataset can be found under `./datasets/Readme.txt`

[Download](https://ora.ox.ac.uk/objects/uuid:03ba4b01-cfed-46d3-9b1a-7d4a7bdf6fac/files/m5ac36a1e2073852e4f1f7dee647909a7) the datasets before training and testing, and put the file `Oxford_Battery_Degradation_Dataset_1.mat` under `./datasets`.

### Setup

To set up the project, create a virtual environment based on Python 3.10 with Jupyter-Notebook. Activate the virtual environment and run:

```
pip install -r requirements.txt
```

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Credit

This project use open source library [Pytorch](https://pytorch.org/) to build the model.

## Acknowledgement 

This project is licensed under the [MIT LICENCE](https://github.com/sileneer/NRP_2022_EEE12/blob/main/LICENCE)

We appreciate David Howey and Christoph Birkl for their work in collecting the datasets `Oxford_Battery_Degradation_Dataset_1`, and their research at https://scholar.google.co.uk/citations?hl=en&user=AZdBXIkAAAAJ&view_op=list_works&sortby=pubdate. 

[1] Christoph R. Birkl, "Diagnosis and Prognosis of Degradation in Lithium-Ion Batteries", PhD thesis, Department of Engineering Science, University of Oxford, 2017. 
