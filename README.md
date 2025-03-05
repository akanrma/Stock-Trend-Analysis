# Stock-Market-Trend-Analysis-Using-HMM-LSTM

Update: There is new version of this project, see more details on https://github.com/Yikiwi13/HMM-GMM-Timing-Strategy.git

## Introduction

The hidden Markov model (HMM) is a signal prediction model which has been used to predict economic regimes and stock prices. This project intends to achieve the goal of applying machine learning algrithms into stock market. The long short term memory model (LSTM) ensures that the previous information can continue to propagate backwards without disappearing as the hidden layer continuously superimposes the input sequence under the new time state.Our main purpose is to predict the ups and downs of one stock by using HMM-LSTM.<br> 
See details in our paper: [PAPER](https://arxiv.org/abs/2104.09700)

## Process
 
Using data from 2007-2018 in China's A share stock market, including daily price and trade volume and over 200 types of feature, we divided them into 8 types of features and make 8 HMMs. Then combined them together to predict ups and downs of stock price the next day. During which, we used GMM and XGBoost to fit the emission matrix B of continuous HMMs and used LSTM to find a better connection of X and Y. Moreover, an useful method of labeling called the reiple barrier method is well used to find relationship between hidden states and the trends of stock price.<br>
 
 ```
  `
 
### Experiment with 4 different models: <br>
 
 * #### GMM-HMM <br>
 * #### XGB-HMM <br>
 * #### GMM-HMM-LSTM <br>
 * #### XGB-HMM-LSTM <br>
 
 ### Compared with the results: <br>

* #### train_set

![](https://github.com/JINGEWU/Stock-Market-Trend-Analysis-Using-HMM-LSTM/raw/master/FIGURE/train1.jpg)  

* #### test_set

![](https://github.com/JINGEWU/Stock-Market-Trend-Analysis-Using-HMM-LSTM/raw/master/FIGURE/test1.jpg)  

* #### iteration_process

![](https://github.com/JINGEWU/Stock-Market-Trend-Analysis-Using-HMM-LSTM/raw/master/FIGURE/best_iter.png)  

* #### Accuracy
   GMM-HMM-LSTM performs 76.1612738% <br>
   XGB-HMM-LSTM performs 80.6991611% <br>

## Contribution

### Contributors

* #### Junbang Huo
* #### Yulin Wu
* #### Jinge Wu

### Institutions

* #### AI&FintechLab of Likelihood Technology
* #### Sun Yat-sen University
* #### Xi'an Jiaotong-Liverpool University

## Acknowledgement

We would like to say thanks to Maxwell Liu from ShingingMidas Private Fund, Jiahui Wu and Xingyu Fu from Sun Yat-sen University for their generous guidance throughout the project

## Set up

### Python Version

* #### 3.6

### Modules needed

* #### numpy
* #### pandas
* #### hmmlearn
* #### xgboost
* #### ...

## Contact
Please contact Mingwen Liu(刘铭文) liumwen@shiningmidas.com for more information about data.
* liumwen@shiningmidas.com
* huojb3@mail2.sysu.edu.cn
* wuylin6@mail2.sysu.edu.cn
* jinge.wu@outlook.com
