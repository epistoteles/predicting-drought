<h1 align="center">🌧️ Predicting Droughts ☀️</h4>

<p align="center">
  <a href="#-why-predict-droughts">Why</a> •
  <a href="#%EF%B8%8F-installation">Installation</a> •
  <a href="#-benchmarks">Benchmarks and Results</a> •
  <a href="#%EF%B8%8F-license">License</a>
</p>

ABC

## 🤔 Why Predict Droughts?

Droughts are becoming more frequent and more severe.

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

The following benchmarks:

| Model | Macro F1 Mean | MAE Mean |
| --- | --- | --- |
| Random guessing | 0.108 | 2.244 |
| Majority class | 0.133 | 0.578 |
| Random guessing (stratified) | 0.164 | 1.046 |
| LSTM ([@MiniXC](https://github.com/MiniXC)) | 0.639 | 0.277 |

An up-to-date benchmark list of all handed in models can be found in the original kaggle task: https://www.kaggle.com/cdminix/us-drought-meteorological-data/tasks?taskId=3422.

## ⚠️ License
This repository has been published under the MIT license.
