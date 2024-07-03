The app is intended to help people with Autism, where their voices are hard to understand for general public, yet still recognizable to parents/siblings. To achieve such task, we use google TFLite model maker to retrain with voices of specific individual, then use Google's MediaPipe for audio classification. 
1. modelMaker uses customized voice data to generate model data
2. app uses generated model data to recognize voices of the same person.

## Setup
You need to have python 3.9 to run app and modelmaker. Here I cover setup for windows
1. Install WSL2 for windows with Ubuntu 22.04 LTS.
2. in WSL2, install brew with the following command.
    ```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```
4. Install VSCode for WSL2.
5. Install anaconda in wsl2:
6. ```
7. wget https://repo.anaconda.com/archive/Anaconda3-2022.10-Linux-x86_64.sh
8. bash Anaconda3-2022.10-Linux-x86_64.sh
9. ```
Install Jupeter Notebook in WSL2
```
sudo ufw allow from any to any port 8888 proto tcp
   jupyter notebook --generate-config
   cd .jupyter
   nano jupyter_notebook_config.py
```   
