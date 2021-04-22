# federated-emotion
This repo contains the code and paper for implementing a Federated Learning system to classify emotions in speech. The description of the experiments ran and the results of such experiments are contained in the paper.

## Datasets Used:
 - IEMOCAP: multi-modal and multi-speaker database that contains approximately 12 hours of audiovisual data - video, speech, and text transcriptions. The data-set contains utterances for 10 speakers divided into 9 emotions (anger, happiness, excitement, sadness, frustration, fear, surprise, other and neutral state). For our experiments, we only utilize 4 emotions (anger, excitement, sadness, and neutral) as all the other emotions have less than 100 utterances.

## Structure of the Code
All the code is contained in three different notebooks contained inside the notebook directory:
  1. PDL_Project_Baseline_CPU - which contains the code for reading, pre-processing the audio and training all the architectures on a CPU with a centralized system
  2. PDL_Project_Baseline_GPU - which contains the code for reading, pre-processing the audio and training all the architectures on a GPU with a centralized system
  3. PDL_Project_Federated - which contains the code for reading, pre-processing the audio and training all the architectures in a federated manner utilizing the two data distribution discussed in the paper.
All the notebooks were run in Google Colab for simplicity, but they could be run in any environment as long as the user install tensorflow-federated and any other packgae that is imported in the notebook that is not already included in their environments by default (numpy, pandas, and matplotlib).

## Structure of the Docs
The docs directory contains the paper with all the information about the experimental setup and the required background information. It also includes the slides for the presentation given in class.
