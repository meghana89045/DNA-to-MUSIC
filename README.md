# DNA-to-MUSIC

#  DNA2Music – Deep Learning Based DNA to Music Generation

##  Project Overview

**DNA2Music** is a deep learning–based project that converts **DNA sequences into music**.
By learning patterns in genetic data using advanced neural networks, the system generates **unique musical compositions (MIDI files)** from DNA sequences.

This project brings together:

* 🧬 Bioinformatics
* 🤖 Deep Learning
* 🎼 Algorithmic Music Generation


##  DNA to Music Mapping

DNA sequences consist of four nucleotides:

| Nucleotide | Encoding |
| ---------- | -------- |
| A          | 0        |
| T          | 1        |
| C          | 2        |
| G          | 3        |

Process:

1. DNA → Numeric encoding
2. Numeric values → Musical notes
3. Position + value → Note duration
4. Output → **MIDI music file**


## Models Implemented

This project compares multiple deep learning architectures:

###  CNN (Convolutional Neural Network)

* Extracts local DNA patterns
* Fast and efficient

###  LSTM

* Captures long-term dependencies in DNA sequences

###  Hybrid CNN–LSTM

* CNN for feature extraction
* LSTM for temporal learning

###  Bidirectional LSTM

* Processes DNA both forward and backward
* Improved contextual understanding

###  GRU Models

* GRU
* Bidirectional GRU
* Stacked GRU
* Faster training with good accuracy

###  Transformer

* Multi-head self-attention
* Captures global sequence relationships

###  Vision Transformer (ViT)

* DNA divided into patches
* Transformer attention applied on DNA segments

###  Swin Transformer (CNN-inspired Transformer)

* Hierarchical feature learning
* Efficient long-sequence processing

##  Project Structure

```
DNA2Music/
│
├── deeplearning_project_dna2music.py
├── deeplearning_project_DNA2MUSIC.ipynb
│
├── training_curves.png
├── confusion_matrices.png
├── bidirectional_training_curves.png
├── bidirectional_confusion_matrices.png
│
├── model_parameters.csv
├── model_performance_metrics.csv
│
├── dna_music_pair_*.mid
├── bidirectional_dna_music_*.mid
├── transformer_music_*.mid
├── vit_music_*.mid
│
└── README.md
```


##  Requirements

Install dependencies using:

```bash
pip install numpy pandas matplotlib seaborn
pip install tensorflow scikit-learn
pip install biopython music21
```

> `music21` is required for MIDI generation.


##  How to Run

###  Using Python Script

```bash
python deeplearning_project_dna2music.py
```

### Using Jupyter Notebook

Open and run:

```text
deeplearning_project_DNA2MUSIC.ipynb
```

(Recommended on **Google Colab**)

##  Dataset

* Accepts **FASTA DNA files**
* Filters invalid nucleotides automatically
* Uses sliding windows for training
* Generates synthetic DNA sequences if no FASTA file is provided

## Evaluation Metrics

Models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Trainable vs Non-trainable parameters

Results are saved as:

* `.png` plots
* `.csv` tables

##  Music Generation

Each trained model generates:

*  MIDI music files
* Unique melodies per DNA sequence
* Different rhythmic and tonal structures

Example outputs:

```
dna_music_pair_1.mid
bidirectional_dna_music_2.mid
transformer_music_1.mid
vit_music_3.mid
```


##  Observations

* **Bidirectional LSTM** performs consistently well
* **Transformer models** capture global DNA patterns
* **Hybrid CNN–LSTM** offers a balance between speed and accuracy


##  Applications

* Bioinformatics visualization
* Educational genomics tools
* AI-generated music
* Computational biology research
* Creative AI projects


##  Future Enhancements

* Real biological genome datasets
* Emotion-based music mapping
* Audio waveform generation
* GAN-based music synthesis
* Real-time DNA-to-music conversion



##  License

This project is intended for **academic and research use**.
You are free to use and modify it with proper attribution.

