# Conversational AI using Seq2Seq with Attention
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Framework](https://img.shields.io/badge/Framework-PyTorch-red)
![Status](https://img.shields.io/badge/Project-Research%20Implementation-green)

This repository contains the implementation of a Conversational AI chatbot using a Sequence-to-Sequence (Seq2Seq) neural network with attention mechanisms built using PyTorch. The model is trained on the Cornell Movie Dialog Corpus to generate human-like responses in a dialogue setting.

This work is based on our published research paper presented at the International Conference on Computing and Machine Learning (CML 2025) and published in Springer's Lecture Notes in Networks and Systems series.

---------------------------------------------------------------------

## Published Research Paper

This project is associated with the following peer-reviewed publication.

Upadhye, S. V., Mullalli, T. S., Neha, R., Karuna, A. K., Hegde, S., Dhulavvagol, P. M. (2026).  
Enhancing Dialogue Systems with Attention Mechanisms: Conversational AI Using Seq2Seq.

In Bansal, J. C., Borah, S., Hussain, S., Salhi, S. (eds) Computing and Machine Learning (CML 2025).  
Lecture Notes in Networks and Systems, vol 1613. Springer, Singapore.

DOI  
https://doi.org/10.1007/978-981-95-2875-2_22  

Springer Link  
https://link.springer.com/chapter/10.1007/978-981-95-2875-2_22

---------------------------------------------------------------------

## Project Overview

Conversational AI systems aim to simulate natural human dialogue. This project builds a chatbot model using deep learning techniques including

- Sequence to Sequence neural networks  
- Attention mechanisms  
- Encoder Decoder architecture  
- Natural language preprocessing  
- Dialogue dataset training  

The model learns conversational patterns from movie dialogues and generates context aware responses.

---------------------------------------------------------------------

## Dataset

The model is trained using the Cornell Movie Dialog Corpus which contains

- Large collection of fictional conversations  
- Movie character dialogue pairs  
- Natural conversational structures  

The dataset is not included in this repository due to size limitations.

You can download it from  
https://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html

After downloading the dataset, place it locally before running the notebook.

---------------------------------------------------------------------

## Methodology

The conversational model follows the following pipeline

1 Data preprocessing  
2 Sentence normalization  
3 Vocabulary construction  
4 Encoder Decoder model creation  
5 Training using dialogue pairs  
6 Response generation  

---------------------------------------------------------------------

## Model Architecture

The chatbot uses a Seq2Seq architecture with attention consisting of two main components.

### Encoder

The encoder reads the input sentence and converts it into a context representation.

Main components

- Embedding layer  
- GRU (Gated Recurrent Unit)  
- Hidden state representation  

The encoder captures the semantic meaning of the input sequence.

### Decoder

The decoder generates the response sentence word by word.

Main components

- Attention mechanism  
- GRU network  
- Output probability layer  

The attention mechanism helps the decoder focus on relevant parts of the input sentence during response generation.

---------------------------------------------------------------------

## Preprocessing Steps

The dataset undergoes several preprocessing steps before training.

These include

- Unicode normalization  
- Lowercasing text  
- Removing non alphabetic characters  
- Tokenization  
- Vocabulary creation  
- Padding sentences  
- Creating input target sentence pairs  

Special tokens used

PAD – padding token  
SOS – start of sentence token  
EOS – end of sentence token  

---------------------------------------------------------------------

## Training Process

The model is trained using PyTorch with the following steps

- Convert sentences to numerical tensors  
- Train encoder and decoder jointly  
- Use teacher forcing during training  
- Compute loss using cross entropy  
- Backpropagation using Adam optimizer  

The model gradually learns conversational patterns and improves response quality.

---------------------------------------------------------------------

## Technologies Used

Programming Language

Python

Libraries

PyTorch  
NumPy  
NLTK  
Matplotlib  

Environment

Google Colab  
Jupyter Notebook

---------------------------------------------------------------------

## Project Structure

Conversational-AI  
│  
├── Conversational_AI_finale.ipynb  
└── README.md  
└── requirements.txt

---------------------------------------------------------------------

## Example Workflow

1 Load the dataset  
2 Preprocess dialogue sentences  
3 Build vocabulary dictionary  
4 Train Seq2Seq model  
5 Generate chatbot responses  

---------------------------------------------------------------------

## Applications

Conversational AI systems like this can be applied in

- Customer support chatbots  
- Virtual assistants  
- Dialogue systems  
- Educational AI tutors  
- Interactive storytelling  

---------------------------------------------------------------------

## Future Improvements

Potential improvements for the system include

- Transformer based conversational models  
- Larger conversational datasets  
- Better response ranking  
- Context memory across multiple turns  
- Deployment as a web chatbot  

---------------------------------------------------------------------

## Citation

If you use this work please cite

Upadhye, S.V., Mullalli, T.S., Neha, R., Karuna, A.K., Hegde, S., Dhulavvagol, P.M. (2026).  
Enhancing Dialogue Systems with Attention Mechanisms: Conversational AI Using Seq2Seq.  
In Bansal, J.C., Borah, S., Hussain, S., Salhi, S. (eds) Computing and Machine Learning.  
CML 2025. Lecture Notes in Networks and Systems, vol 1613. Springer, Singapore.  
https://doi.org/10.1007/978-981-95-2875-2_22

---------------------------------------------------------------------

## Author

Shreya Vijaykumar Upadhye  
Bachelor of Engineering in Computer Science  
KLE Technological University, India

Research Interests

Artificial Intelligence  
Conversational AI  
Natural Language Processing  
Machine Learning
