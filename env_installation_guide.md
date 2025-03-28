# Environment Installation Instructions

In this instruction, we will use the scientific Python distribution “conda” (https://docs.conda.io/en/latest/) with fully open-source packages from https://conda-forge.org/. 

Follow the instructions according to your operating system.

## MS Windows

1. Download the miniforge windows installer: https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe
2. Execute the installer and follow the instructions. Please use the default settings.
3. Test if installation was successful, by opening the programme "Miniforge Prompt" and see if *conda* outputs the options of conda
4. Download the following [environment.yml](https://github.com/OpenSenseAction/TrainingSchoolEnvIntro/blob/main/environment.yml) file.
5. Open the program called “Miniforge Prompt”
6. In the command line of “Miniforge Prompt” navigate to the repository downloaded in (4) to the location of the downloaded file “environment.yml” by using e.g. cd C:/User/username/Download/. (If you are not yet familiar with the command line, you can have a look at [this tutorial](https://www.digitalcitizen.life/command-prompt-how-use-basic-commands/))
7. When you are in the same directory as the downloaded “environment.yml” file, execute the following command on the command line: *conda env create --file environment.yml*
    Note that it may take several minutes till conda calculates which package versions to download. After some minutes you will be presented with a list of Python packages that have to be downloaded. In case the installation does not start, you might need to select “yes” or press Return to start the download and installation.
8. Activate the environment via the command *conda activate opensense_training*
9. Clone the codebase for this intro with *git clone https://github.com/OpenSenseAction/TrainingSchoolEnvIntro.git*
10. cd to the directory of the repository (*cd TrainingSchoolEnvIntro*)  
11. Start jupyterlab (the programming environment that we will use during the workshop) by executing the following command on the command line: *jupyter-lab --no-browser* copy one of the last two localhost URLs to your favorite web browser (Chrome is recommended for Jupyterlab, we have not tested with Edge but it should also work)
12. Open one of the notebooks from scentific_python and execute the first few cells by clicking the play button at the top of the notebook. If all cells are executed without a red error message, you are setup!
    
## Linux/MacOS

1. Download mamba-forge according to your Operating System: https://github.com/conda-forge/miniforge?tab=readme-ov-file#unix-like-platforms-macos--linux
2. Locate the installer shell script in your terminal and run it. Use the default options. Do not change any of the default settings unless you are an expert for using conda and know how to set up conda and conda environments!
3. Download ([instructions for downloading](https://docs.github.com/en/repositories/working-with-files/using-files/downloading-source-code-archives#downloading-source-code-archives)) or clone ([instructions for cloning](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)) this [repository](https://github.com/OpenSenseAction/TrainingSchoolEnvIntro). The usage of cloning and git is encouraged! If you still need to install git find the instructions [here](https://github.com/git-guides/install-git).
4. Navigate to the repository downloaded in (3) to the location of the downloaded file “environment.yml” by using e.g. *cd C:/User/username/Download/* (If you are not yet familiar with the command line, you can have a look at [this tutorial](https://www.digitalcitizen.life/command-prompt-how-use-basic-commands/))
5. When you are in the same directory as the downloaded “environment.yml” file, execute the following command on the command line: *conda env create -f environment.yml* Note that it may take several minutes till conda calculates which package versions to download. After some minutes you will be presented with a list of Python packages that have to be downloaded. In case the installation does not start, you might need to select “yes” or press Return to start the download and installation.
6. Activate the environment via the command *conda activate opensense_training*
7. Start jupyterlab (the programming environment that we will use during the workshop)
   *jupyter-lab --no-browser* copy one of the last two localhost URLs to your favorite web browser (Chrome is recommended for Jupyterlab). 
8. Open one of the notebooks from scentific_python and execute the first few cells by clicking the play button at the top of the notebook. If all cells are executed without a red error message, you are setup!
