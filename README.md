# eeg-mental-state-classification
EEG brainwave mental-state classification using Random Forest to practice what I have learned ffrom my ML tutorials.

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

- [5] numpy, pandas and matplotlib is already built-in but wanted to verify.
- [11] learned to transfer the data-set fom kaggle to colab
- [20] getting to know the data as well as visualising it 
- [45] labels and features
- [46] spliting data to train-test
- [47] training w 100 estim
- [48] testing how good it learned : seems %100
- [49] testing the general accuracy : 0.96...
- [51] is it accurate for every feature? : %96 accurcy, neutral was harder to guess bcs of the blurred line between neautral-other feature
- [53] confusion matrix : 
   relaxed : 160 ✅ 
   neutral : 155 ✅ 
   concentrating : 162 ✅ |°|
   6 relaxed -> was considered neutral |°|
   12 neutral -> was considered concentrating
   




