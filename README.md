# deep-emotion-sense
Convolutional neural network to predict language-independent emotion on a dataset of English and French speech. 

This model is trained on a merged dataset of natural speech with data provided by [IEMOCAP](https://sail.usc.edu/iemocap/ "The Interactive Emotional Dyadic Motion Capture (IEMOCAP) Database") for english speech samples and [Recola](https://recola.hepforge.org/ "Recola: Recursive Computation of 1-Loop Amplitudes") for french speech samples.

The implementation is a basis for a [research paper on comparison on different optimization algorithms and activation functions](https://github.com/nymvno/Emotion-Recognizer/blob/master/Language-independent%20Emotion%20Recognition%20from%20Speech.pdf "Language-independent Emotion Recognition from Speech").

## Getting Started
You can view the notebook [here](https://github.com/nymvno/EmotionRecognizer/blob/master/CNN%20SpeechRecognition.ipynb).
### Run the notebook
#### Prerequisites
- Python 3
- Tensorflow

#### Starting the notebook
Simply open a new terminal in the directory and type:
```bash
> jupyter notebook
```

## Built With

* [Tensorflow](https://www.tensorflow.org/)

## Contributors

* **F. Strohm** - [StrohmFn](https://github.com/StrohmFn)
* **C. Tasci** - [StraysWonderland](https://github.com/StraysWonderland)

## Experimental Results

### Englisch testset

|Class | Mono-lingual | Multi-lingual | Cross-language
|:--|:--|:--|:--|
|Sadness | 0.000 | 0.015| 0.015
|Anger |0.019 |0.014| 0.014
|Pleasure| 0.043 |0.010| 0.120
|Joy| 0.942| 0.985| 0.864
|MICRO| 0.421| 0.432| 0.405

### French testset

Class | Mono-lingual | Multi-lingual | Cross-language
:--|:--|:--|:--|
Sadness| 0.070 |0.000 |0.230
Anger| 0.200 |0.200 |0.200
|Pleasure| 0.350 |0.035 |0.357
Joy| 0.754| 0.912 |0.403
MICRO| 0.533 |0.524 |0.359
