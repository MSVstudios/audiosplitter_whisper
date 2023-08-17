## from https://github.com/JarodMica/audiosplitter_whisper

# Audio Splitter using Whisperx
Created with the purpose for curating datasets for the sake of training AI models.  This is created with RVC (Retrieval-based Voice Conversion) in mind but generally works for any other AI voice model that needs short clips less than 10s.

## Youtube Video Tutorial
https://youtu.be/9lsSSPnF67Q

## Prerequisites
- Python 3.10 installation
- git installation
- vscode installation (highly recommended)
- ffmpeg installation
- Cuda Capable Nvidia GPU (highly recommended)

## Installation and basic usage
1. create Anaconda env
```
conda create --name audiosplitter_whisper python=3.10
```

2. activate Ancaond virtual env
```
conda activate audiosplitter_whisper 
```

3. Clone the repository (repo)
```
git clone https://github.com/MSVstudios/audiosplitter_whisper.git
```

4. Navigate into the repo with:
```
cd audiosplitter_whisper
``` 

5. install torch (latest for NVIDIA) https://pytorch.org/get-started/locally/ be careful you must use the Cuda toolkit version as you use in PyTorch: if you use Cuda toolkit 12.1 with PyTorch cuda11.8 you will crash often. In case you have the latest NVidia driver that automatically installs Cuda toolkit 12.1 you can install manual Cuda toolkit 11.8 
```
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

6. install whisperX https://github.com/m-bain/whisperX
```
pip install git+https://github.com/m-bain/whisperx.git
```

7. other requierement
```
pip install -r requirements.txt
```

8. run audio splitter script
```
python split_audio.py
```
