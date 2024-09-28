# AudioCraft Tool

## Description
AudioCraft is an audio processing tool that allows users to download audio from YouTube or Google Drive, separate vocals from instruments, remove silence, and split cleaned audio into manageable chunks. Ideal for musicians and content creators, it streamlines audio manipulation for high-quality results in an easy-to-use format.

## Features
- **Audio Download**: Easily download audio tracks from YouTube or Google Drive.
- **Vocal Separation**: Utilize Demucs to separate vocal tracks from instrumental or noise components.
- **Silence Removal**: Automatically detect and remove silent segments from vocal tracks.
- **Audio Chunking**: Split cleaned audio into smaller, manageable segments based on specified parameters.
- **Google Drive Integration**: Save results directly to Google Drive for easy access and storage.
- **Flexible Input Sources: Download audio directly from YouTube or use audio files stored on Google Drive.
- **Customizable Parameters: Adjust settings like silence threshold, chunk length, and more to suit your specific needs.

## How to Use

### Try it on Colab
[![Open in Colab](https://camo.githubusercontent.com/96889048f8a9014fdeba2a891f97150c6aac6e723f5190236b10215a97ed41f3/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/github/codermillat/AudioMasterTool/blob/main/AudioCraft.ipynb)

### Step 1: Install Dependencies
Make sure you have Python installed, then install the required libraries using:
```bash
pip install yt_dlp ffmpeg-python demucs pydub numpy librosa soundfile
```

### Step 2: Clone the Repository
Clone this repository to your local machine using:
```bash
git clone https://github.com/codermillat/AudioMasterTool.git
cd AudioCraft
```

### Step 3: Mount Google Drive (if using Google Drive)
In your notebook, run:
```python
from google.colab import drive
drive.mount('/content/drive')
```

### Step 4: **Configure Input Parameters**
   - **Mode**: Choose the operation mode (e.g., "Splitting").
   - **Dataset**: Select the source of your audio (`"Youtube"` or `"Drive"`).
   - **URL**: If using YouTube, provide the video URL.
   - **Drive Path**: If using Drive, specify the path to your audio file.
   - **AUDIO_NAME**: Assign a name to your audio file for processing.

### Step 5: Run the Notebook
Execute the cells in the notebook step by step to download the audio, separate vocals, remove silence, and split the audio into chunks.

### Step 6: Access Your Results
Your processed audio files will be saved in your Google Drive or in the designated output folder.

## Acknowledgments
- **Demucs**: For the vocal separation model.
- **yt-dlp**: For downloading audio from YouTube.
- **Pydub**: For audio manipulation and silence detection.
- **Librosa**: For audio processing and analysis.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue for any enhancements or bugs.

## Contact
For questions or suggestions, please reach out via [email](mailto:codermillat@gmail.com).
