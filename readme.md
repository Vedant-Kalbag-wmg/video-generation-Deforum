# Deforum for SageMaker

Instructions to use this repo:
1. Open the terminal from the Launch page
2. Run ```chmod +x ./setup.sh``` to give permissions to run the setup shell script
3. Run ```./setup.sh``` to create and set up the conda environment to be used within the notebook
4. Open ```Deforum_AWS.ipynb``` and select the ```conda_deforum``` kernel
5. Make required modifications to the *first paragraph* and hit run all (This can take quite a while - It takes about 7 seconds per frame to generate, and then upto 5 minutes to generate the video from the images)



Folder structure (after running the notebook, as some files/folders will be created during the run):
```
video-generation-Deforum
├── audio.wav                             -> This file will be auto-downloaded based on the youtube link provided
├── configs                               -> Deforum config files
├── Deforum_AWS.ipynb                     -> Main notebook (RUN THIS)
├── PromptGeneration.ipynb                -> Notebook used to generate variations for a prompt based on creative style, subject and object combinations
├── deforum-stable-diffusion              -> Repo for deforum 
├── environment.yml                       -> Used to create the conda env / notebook kernel
├── readme.md                             -> Setup and run instructions
├── requirements.txt                      -> Python requirements
├── resources                             
│   ├── models                            -> Path where weights and checkpoints are downloaded to
│   └── outputs                           -> OUTPUT PATH FOR GENERATED PHOTO/VIDEO
├── setup.sh                              -> Shell script used to set up the environment
├── source_separated                      -> Created when running demucs to extract stems
│   └── htdemucs_ft
└── start_env.sh                          -> IGNORE, UNUSED

```
