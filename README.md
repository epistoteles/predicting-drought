<h1 align="center">🌧️ Predicting Drought ☀️</h4>

<p align="center">
  <a href="#-why-predict-droughts">Why</a> •
  <a href="#%EF%B8%8F-installation">Installation</a> •
  <a href="#-benchmarks">Benchmarks and Results</a> •
  <a href="#%EF%B8%8F-license">License</a>
</p>

This repository is a code submission for the Master's course 'Machine Learning' at the University of Hamburg.

It explores the usage of [MiniROCKET](https://arxiv.org/pdf/2012.08791.pdf)-transformed features and different classification and regression techniques and performs analyses on feature and history importance.

## 🤔 Why Predict Droughts?

Droughts are becoming [more severe and more frequent](https://www.nature.com/articles/s41598-020-68872-9). 

Even though the prediction of droughts does not prevent them or make them less harmful, it allows countries, cities or individuals to adjust and take preventive measures.

The prediction of droughts may also allow us to better understand influencing factors of droughts.

## ⚙️ Installation

First, you have to download the data from https://www.kaggle.com/cdminix/us-drought-meteorological-data.

Simply place the four files `test_timeseries.csv`, `train_timeseries.csv`, `validation_timeseries.csv` and `soil_data.csv` directly into the main directory.

Next, run the jupyter notebook by navigating into the directory in your terminal and typing
```
jupyter notebook
```

That's it! 🎉 You are ready to go.
All relevant requirements will be installed in the notebook itself.

Executing all cells of the notebook will take about 6 hours.

If you don't have javascript widgets enabled in Jupyter and encounter the error `widget javascript not detected. it may not be installed or enabled properly.`, try running the following commands before starting the notebook:
```
sudo jupyter nbextension enable --py --sys-prefix widgetsnbextension
```
```
jupyter nbextension enable --py widgetsnbextension
```

## 📊 Benchmarks

The following performance benchmarks were either given or achieved:

| Model | Macro F1 Mean | MAE Mean |
| --- | --- | --- |
| Random guessing | 0.108 | 2.244 |
| Majority class | 0.133 | 0.578 |
| Random guessing (stratified) | 0.164 | 1.046 |
| Ridge regression (MiniROCKET features) | 0.444 | 0.372 |
| Ridge regression (default features) | 0.579 | 0.255 |
| LSTM ([@MiniXC](https://github.com/MiniXC)) | 0.639 | 0.277 |

An up-to-date benchmark list of all handed in models can be found in the original kaggle task: https://www.kaggle.com/cdminix/us-drought-meteorological-data/tasks?taskId=3422.

## ⚠️ License
This repository has been published under the MIT license.
