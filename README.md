# eeg-mental-state-classification
EEG brainwave mental-state classification using Random Forest to practice what I have learned ffrom my ML tutorials.

**Research**:

https://jordanjamesbird.com/publications/A-Study-on-Mental-State-Classification-using-EEG-based-Brain-Machine-Interface.pdf

**Dataset**:

- EEG Brainwave Dataset(Kaggle)

**Libraries**
- Pandas
- numpy
- matplotlib
- scikit-learn

**Model** : 
- Random Forest Classifier


**My Notes**

My goal is to train the model to read the mental states from EEG headband signals, so I can automatically classify if the person is relaxed, neutral or concentrating. 

- [] numpy, pandas and matplotlib is already built-in but wanted to verify.
- [] learned to transfer the data-set fom kaggle to colab
- [] getting to know the data as well as visualising it 
- [] labels and features
- [] spliting data to train-test
- [] training w 100 estim
- [] testing how good it learned : seems %100
- [] testing the general accuracy : 0.96...
- [] is it accurate for every feature? : %96 accurcy, neutral was harder to guess bcs of the blurred line between neautral-other feature
- [] confusion matrix : 
   relaxed : 160 ✅ 
   neutral : 155 ✅ 
   concentrating : 162 ✅ |°|
   6 relaxed -> was considered neutral |°|
   12 neutral -> was considered concentrating
- [] trying to analyse freq. features -> the research paper:
     - std -> standard deviation
     - kurt -> kurtosis
     - eigenval -Y
     - logcovM -> log-covariance matrix
     - lag1_ -> 1 sec del()lag
     - freq_122 -> FFT
     - _0, _1, _2, _3-> TP9; AF7; AF8; TP10
     - 5 frq. band : alpha, beta, theta, delta, gemma
 - [] AF8 (right frontal lobe) is the most dominant electrode with 12 / 20 top features, which is associated with concentration
 - [] The most important feature is eigenval_0(TP9 electrode) w 2.9%




