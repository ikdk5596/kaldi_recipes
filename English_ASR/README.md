# English_ASR: Korean Automatic Speech Recognition  
                                                    Hyungwon Yang
                                                    2016.11.12
                                                    EMCS lab    

It is working on Mac(El Capitan) and Ubuntu(14.04).
To run this program, kaldi should be installed on your computer.

### PREREQUISITE

1. **Install Kaldi**
- Type below in command line.
- $ git clone https://github.com/kaldi-asr/kaldi.git kaldi --origin upstream
- $ cd kaldi
- $ git pull 
- Read INSTALL and follow the direction written there.

2. **Install Packages**
- Install list: Sox, coreutils.
-  On mac
- $ brew install sox
- $ brew install coreutils

3. **Unzip language model files.**
- Due to the size of librispeech model files, "HCLG.fst" and "final.mdl" have been zipped. Please unzip them before run the asr code.

### DIRECTION

1. Navigate to 'English_ASR' directory.
2. Open run_asr.sh with any text editor to specify user path of kaldi directory.
- Change 'kaldi' name variable. (initial setting: kaldi=/home/kaldi)
3. Run the code by selecting one of the language models. 
- Two language models are provided: timit and librispeech. 
- ex) $ sh run_asr.sh (language model)
-     $ sh run_asr.sh librispeech
4. You may see the recording status on the screen. Speak any sentence and stop recording by pressing Control + C.
4. Speech recognition process will be automatically initiated and a text result will be printed on the screen.

### CONTACTS
---
Please report bugs or provide any recommendation to us through the following email addresses.

Hyungwon Yang / hyung8758@gmail.com
### VERSION HISTORY
- v.1.0(11/12/16): Two language models are available: timit and librispeech.
