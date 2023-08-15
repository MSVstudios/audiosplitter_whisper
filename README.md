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

pip


6. If you ran into any permission issues, you'll need to change your windows Execution Policy to Remote Signed.  This does lower security on your system a small bit as it allows for scripts to be ran on your computer, however, only those signed by a Trusted Publisher or verified by you can be run (to my knowledge).  Do at your own risk.
    - Open a powershell window as admin.  Then, run the following command:

    ```
    Set-ExecutionPolicy RemoteSigned
    ```

    - If you want to change it back, you can with:
    ```
    Set-ExecutionPolicy Restricted
    ```

7. Now rerun step 5 and activate your venv.  After it's activated, you can then run the following command to start up the script:
```
python split_audio.py
```

For more details, please refer to the youtube video.
