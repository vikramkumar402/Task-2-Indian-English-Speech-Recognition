# Task-2 Indian English Speech Recognition

Task-2 focuses on evaluating a speech recognition algorithm on the "AI4Bharat-NPTEL2020-Indian-English-Speech-Dataset." This project uses the Wav2Vec2 model to convert speech from various Indian accents into text, aiming to measure and improve the accuracy of speech recognition systems on Indian English accents.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Setup and Installation](#setup-and-installation)
- [Running the Project](#running-the-project)
- [Dataset](#dataset)
- [Tools and Technologies](#tools-and-technologies)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Speech-to-Text Conversion**: Utilizes the Wav2Vec2 model for transcribing Indian English speech.
- **AI4Bharat Dataset**: Evaluates model performance on a dataset specifically containing various Indian accents.
- **Detailed Evaluation**: Measures the performance using the Word Error Rate (WER) metric.

## Prerequisites

- Python 3.x
- torchaudio
- transformers
- jiwer

## Setup and Installation

### Clone the Repository

```bash
git clone https://github.com/vikramkumar402/Task-2-Indian-English-Speech-Recognition.git
cd Task-2-Indian-English-Speech-Recognition
```

### Installation

Install the required Python packages using the following commands:

```bash
pip install torch torchaudio librosa transformers jiwer
```

## Running the Project

You can execute the notebook or Python script either locally or using Google Colab for a cloud-based execution environment.

### Running on Google Colab

Click the button below to open the Jupyter notebook in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vikramkumar402/Task-2-Indian-English-Speech-Recognition/blob/main/TASK_2.ipynb)

### Local Setup

If you prefer to run the project locally, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/vikramkumar402/Task-2-Indian-English-Speech-Recognition.git
   cd Task-2-Indian-English-Speech-Recognition
   ```

2. **Install Dependencies**:

   ```bash
   pip install torch
   pip install torchaudio
   pip install librosa
   pip install transformers
   pip install jiwer
   ```

3. **Run the Script**:

   ```bash
   python task_2.py
   ```

## Dataset

This project leverages the *AI4Bharat-NPTEL2020-Indian-English-Speech-Dataset*, a comprehensive collection of Indian English speech recordings. This dataset is specifically designed to capture the diversity of Indian English accents, providing a valuable resource for developing and evaluating speech recognition models.

### Dataset Details:

- *Source*:  NPTEL-HRD YouTube (Playlist) -  Derived from various Indian English speakers.
- *Variety*: For this project, the following subset is used:
  - *Sample Data (Pure-Set)*: This subset includes a variety of accents and more complex audio scenarios.

### Usage in the Project:

The AI4Bharat dataset was integral to developing and testing the speech recognition model. Using the "Pure-Set" subset allowed for a thorough evaluation of the model's accuracy across varying audio conditions:

- *Loading files*: 100%
  - `1000/1000 [00:26<00:00, 58.71it/s]`
- *Loaded 998 valid audio files.*
- *Processing audio*: 100%
  - `998/998 [1:39:14<00:00, 3.80s/it]`
- *Word Error Rate (WER)*: `0.274513`

This structured use of the dataset helps in pinpointing the strengths and limitations of the speech recognition model, providing clear pathways for further enhancements.

## Tools and Technologies

<table>
  <tr>
    <th>Area</th>
    <th>Tool/Technology</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Speech Recognition</td>
    <td>Wav2Vec2 (facebook/wav2vec2-large-960h-lv60-self)</td>
    <td>Used for accurate speech-to-text conversion.</td>
  </tr>
  <tr>
    <td>Audio Processing</td>
    <td>torchaudio, librosa</td>
    <td>Handle audio file processing and manipulation.</td>
  </tr>
  <tr>
    <td>Programming Language</td>
    <td>Python</td>
    <td>The core language used for developing the application.</td>
  </tr>
</table>




## Results

The performance of the speech recognition model was evaluated using the Word Error Rate (WER), which is a common metric in speech recognition that measures the minimal number of word insertions, deletions, and substitutions required to change the recognized text into the reference text.

| Dataset                | Average WER |
| ---------------------- | ----------- |
| Sample Data (Pure-Set) | 0.274513    |

These results indicate the accuracy level of the transcription of audio from the AI4Bharat dataset, especially in cleaner audio conditions.

## Conclusion

The Wav2Vec2 model, specifically the facebook/wav2vec2-large-960h-lv60-self variant, demonstrated robust performance in transcribing Indian English accents. The achieved Word Error Rate (WER) of 0.274513 on the Pure-Set subset indicates a reasonable accuracy level for speech recognition tasks in diverse audio conditions.

## Contributing

To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add YourFeature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Create a new Pull Request.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Vikram Kumar - vikramk.ug22.cs@nitp.ac.in

LinkedIn: [linkedin.com/in/vikramkumar2510/](https://www.linkedin.com/in/vikramkumar2510/)

Project Link: [Task-2-Indian-English-Speech-Recognition](https://github.com/vikramkumar402/Task-2-Indian-English-Speech-Recognition)

