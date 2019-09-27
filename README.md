# Stock-Market-Predcition-using-ResNet

## 1. Prepare Environment
pip install arrow
pip install mpl_finance
pip install yfinance
pip install keras==2.2.4
pip install scipy==1.1.0
pip install opencv-python
pip install pandas==0.24.2

## 2. Prepare dataset
To download data, we provide 2 source, yahoo and tiingo (yahoo by default). We can read a list of stock market and run it. Example, we want to download and preprocess all stock market in tw50.csv with 20 period days and produce 50x50 image dimension.

```
$ python runallfromlist.py tw50.csv 20 50
```
Generate the final dataset. Example, we want to generate a final dataset from tw50 with 20 period days and 50 dimension.
```
$ python generatebigdata.py dataset 20_50 bigdata_20_50
```

## 3. Build the model
We can run build model with default parameter.
```
$ python myDeepCNN.py -i dataset/bigdata_20_50
```
