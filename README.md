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
1. use shift+command+p to open the command pallet and select create a jupyter notebook 
2. rename untitled.ipynb to ldooleyeda.ipynb using control + mouse clivk
3. open notebook for editing
4. Use select kernal to choose python environment 3.11.4 newer version doesnt see the modules 

>option2
1. open terminal 
2. start jupyter lab by running - default browser should open to jupyter notebook interface
    '''jupyter lab'''
1.  create new file named ldooleyeda.ipynb.
2.  choose python environment


# 1. Write an introduction to the notebook  
Give introduction a title, author and date. Then a short paragragh on what the notebook is about.
 > '''# = headings''' 
 > ''' <br> = line breaks''' 

# 2. Import Dependencies  
    List python standard libraries Next are the external libraries, then local modules 

# 3. Exloritory Data Analysis.
    Step 1. Data aquistion. Using panda to readd the iris .csv file. print out the first line (heading) of the data set
        ''' # Load the Iris dataset into DataFrame
               df = sns.load_dataset('iris')'''

        ''' # Inspect first rows of the DataFrame
                print(df.head())'''

    Step 2. Initial Data inspection. Display the first 10 rows of the DataFrame, check the shape, and display the data types of each column using df.head(10), df.shape, and df.dtypes.
        '''print(df.head(10))
           print(df.shape)
           print(df.dtypes)'''
    
    step 3.  Initial Descriptive Statistics. Use the DataFrame describe() method to display summary statistics for each column.
        '''print(df.describe())'''

    Step 4. Initial Data Distribution for Numerical Columns. Choose a numerical column and use df['column_name'].hist() to plot a histogram for that specific column. To show all the histograms for all numerical columns, use df.hist().
        '''Inspect histogram by numerical column
            df['sepal_length'].hist()

            # Inspect histograms for all numerical columns
            df.hist()

            # Show all plots
            plt.show()'''
    Document observations in a markdown cell

    Step 5. Initial Data Distribution for Categorical Columns.Choose a categorical column and use df['column_name'].value_counts() to display the count of each category. Use a loop to show the value counts for all categorical columns.
            '''# Inspect value counts by categorical column
                df['species'].value_counts()
               # Inspect value counts for all categorical columns
               for col in df.select_dtypes(include=['object', 'category']).columns:
               # Display count plot
                sns.countplot(x=col, data=df)
                plt.title(f'Distribution of {col}')
                plt.show()'''
    use a markdown cell to document opswrvations.

    Step 6.  Initial Data Transformation and Feature Engineering. Use pandas and other tools to perform transformations as needed. Transformation may include renaming columns, adding new columns, or transforming existing data for more in-depth analysis.
            '''# Renaming a column
               df.rename(columns={'sepal_length': 'Sepal Length'}, inplace=True)

               # Adding a new column
                df['Sepal Area'] = df['Sepal Length'] * df['sepal_width']'''

    Step 7. nitial Visualizations. Create a variety of chart types using seaborn and matplotlib to showcase different aspects of the data. 

    Step 8. Initial Storytelling and Presentation. Present your notebook with an opening that introduces yourself and your topic. Use Markdown section headings to introduce each step. Interpret the visualizations and statistics to narrate a clear and compelling data story. Present your findings in a logical and engaging manner.

# Evaluation Criteria
Functionality: The project should be functional and meet all requirements.
Documentation: The project should be well-written and well-documented.
Presentation: The project should be presented in a clear and organized manner.
Professionalism: The project should be submitted on-time and reflect an original, creative effort.
See rubric for additional information.

# Resources
See JUPYTER.md for Jupyter Notebook keyboard shortcuts and recommendations.
See MARKDOWN.md for Markdown syntax and recommendations.
See Plotting graph For IRIS Dataset Using Seaborn And Matplotlib
See Seaborn Tutorial
Troubleshooting Mac SSL Certificate Error
Seaborn fetches datasets from the web. Newer Macs don't have the required SSL Certificate functionaliy installed by default. There is a post-installation process that must be run. For more information see: MAC-SSL.md.

A


    







