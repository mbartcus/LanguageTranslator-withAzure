# LanguageTranslator-withAzure

## Description of files in the project
- config.json - the configuration used by our program to access the microsoft azure translator
- pydetectlang.py - the main python script that detects the language and prints it
- utils.py - the useful functions to be used in python code
- executable - bash script to run (detecting the language)
- executable_curl - bash script to run curl (detecting the language)
- requerements.txt - the python packages to be installed in your environment
- HELP_USER.txt - this file describes the usage of the program

## Running the program
To run the program for detecting the language you need to:

1. Open the terminal
2. Go to the good directory /project_1
3. Modify executable
	- Give the directory to the dataset containing the labels for each language (the project contains already the good path)
	- Give the text for detecting language
4. In terminal run: 
	./executable > results/result_5most_spoken.txt

## Setting the program
To run the python code you also need to create a hidden .env file in the same directory that contains the following information. If you use a git repository don't forget to add this file to the .gitignore file in order to hide the key from other users.

- API_KEY = <key>
- ENDPOINT = https://api.cognitive.microsofttranslator.com
- LOCATION = francecentral
- PATH_DETECT = /detect

### Setting Permanent Environment Variables in Bash
$ nano /home/user/.bashrc
### Content of the .bashrc file
export KEY_AZURE_for_curl=<key>
