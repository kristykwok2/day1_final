1. Create README.md file for taking notes

## Saving code (syncing with Github repository)
# On the left-hand side of the screen, go to 'source control' (the H looking thing) and press the + next to files to add to the commit
# Add to staged changes
# Enter a commit message (anything)
# Click 'Commit'
# Click 'Sync changes'
# Check GitHub repository to confirm

## Setting up environment (in terminal)
1. Create virtual environment
> python -m venv .venv
2. Activate virtual environment
> source .venv/bin/activate
3. To install libraries/dependencies, first create a requirements.txt file
4. Add OpenAI, Streamlit, and python-dotenv to requirements.txt file
5. Install dependencies by referring to requirements.txt file 
> pip install -r requirements.txt
6. Create a .env file (right click -> new file)
7. Ensure .env file is grayed out (git ignored) - if not, edit .gitignore to include .env
8. Add secrets to .env
> OPENAI_API_KEY = "<insert>"

## Remember to resync with Github repository! 

## Create some code
1. Create a python file - call it what you want - home.py by convention (keep it simple for now, if it gets to like more than 50 lines make a new one)
2. Run streamlit, referring to file you created
> streamlit run bottomtext.py

## Create code in your python file 
1. Import streamlit
> import streamlit as st
2. Import OpenAI
> from openai import OPENAI
3. Import python-dotenv
> from dotenv import load_dotenv
4. Get all of the secrets values
> load_dotenv()