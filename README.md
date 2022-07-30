
# Melody Generation with LSTM in TF2.X

![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

This project focuses on the idea that the audio data is also sequential data where it can be considered as a signal which has modulation with time similarly to the launguage processing data where new word points are collected in a  sequence with time values.

## Results

## Architecture
The model consists of simple LSTM architecture. LSTM refers Long Short Term Memory which stores previous information of data points to predict next data point. So here we have used a simple yet powerfull architecture to predict the next sequence of music notes to generate melody.

## Dataset
File Used map notes to a number : [mapping.json](https://drive.google.com/file/d/1-58w_I8uzKFtp1kVk3DWZvAD9EhCO4al/view?usp=sharing)

full dataset to train Model :[fileDataset](https://drive.google.com/file/d/1-451sk3_bwL2EmU7PRZTYpfCKm_iwb1u/view?usp=sharing)

Trained Model Weights : [model Weights](https://drive.google.com/file/d/1c6-kpE5_aKlw33-bf7-WMvuLko97oP1s/view?usp=sharing)




## Instruction

Open provided file in colab
- Full Train : 
```bash
  set your Paths
  run whole scipt
```
    
- Test : 
```bash
  download provided files
  run only generation part labbel in file
```

## Dependencies
- python
- tensorflow
- numpy 
- music21
- Ipython

## Extras
- for fluid synth installation:
```bash
!apt install fluidsynth
!cp /usr/share/sounds/sf2/FluidR3_GM.sf2 ./font.sf2
```
- convert .midi to .wav
```bash
!fluidsynth -ni font.sf2 {path of midi file wihtout quotes} -F output0.wav -r 44100
IpythonAudio('output.wav')
```  