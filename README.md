# datafun-04-jupyter

# create Repository named datafun-04-jupyter

Option 1

Use GitHub 
1. under repository click new
2. Add repo name
3. Make public 
4. Create README.md file 
5. Add .gitignore file using phython template

# Clone repo in using terminal 
1. open terminal in the documents to store repe
    '''cd documents''
2. clone repo 
    '''git clone https://github.com/Ldooley32/datafun-04-jupyter'''
3. open repo folder using VS code.
4. add requirements.txt
5. Create a virtual environment
    ''' python3 -m venv .venv'''
6. activate environment
    ''' source .venv/bin/sctivate'''
7. push chages to GitHub
    ''' git add .
        git commit -m "informative message"
        git push origin main'''

# add the following to requirements.txt
    '''jupyterlab 
        numpy 
        pandas
        matplotlib 
        seaborn 
        scipy'''
>install the listed libraryies make sure virtual environment is activated
    '''python3 -m pip install -r requirements.txt''

>freeze dependency in the requirements.txt
    '''python3 -m pip freeze > requirements.txt'''

# Start Jupyter in VScode
> Option 1
1. create a file FirstNotebook.ipynb - important to have file extension correct.
2. open file for editing

>option2
1. open terminal 
2. start jupyter lab by running - default browser should open to jupyter notebook interface
    '''jupyter lab'''

# Create a Notebook
1.  create file named TestDrive.ipynb.
2.  use select kernal to chose python environment


