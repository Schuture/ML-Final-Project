# ML-Final-Project

Final project of the course "Introduction to Machine Learning", group members: Yixiong Chen (ychen646), Zuojun Zhou (zzhou111), Susan Wang, (qwang95), Yuhao Zheng (yzhen130).

In this project, we implement and compare popular ML methods for voice recognition for celebrities. It contains two parts: traditional machine learning algorithms, and deep neural networks (including the SOTA models).

## Dataset preperation

We use the [VoxCeleb1](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/vox1.html) dataset ([Google Drive](https://drive.google.com/file/d/1pul2RuYuuw_dFLDRNARDHyhIQqcirQXf/view?usp=sharing)), containing 1211 celebrities, 21,819 videos, and 153,516 audio clips. For illustrating a more powerful result, we only sample 200 speakers for the voice classification task.

## Environment

Please use ```requirements.txt``` to install all the dependencies.

## ML algorithms


## DL algorithms

Please refer to ```DL VoxCeleb analysis.ipynb``` for the DL-based methods. To run this notebook, please modify the data dir to your own dir. And you can download the [pre-extracted vocal features](https://drive.google.com/file/d/11RiR0uAF8rgvOagO3mjqLEjU4Q2nQ42u/view?usp=sharing) and [YAMNet features](https://drive.google.com/file/d/10s6PY_Hlau0HzR32nMr5Q6Ffaq92CJan/view?usp=sharing) to train the models instead of extracting them on your own.
We tired:

- Traditional audio features as the input for MLP models (3 different sizes)
- HuBert Model, which is too large for our computation resource and is abandoned
- Wav2Vec model, a pretrained audio analysis model, reaches the highest performance
- YAMNet, a pretrained sound event detection model, not suitable for speaker identification


