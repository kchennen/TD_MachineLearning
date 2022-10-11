# Machine Learning TD
By Kirsley Chennen & Corentin Meyer @ CSTB - ICube, 11/10 ESBS


# Prerequisite  
In this TD you will learn how to perform a full end-to-end data analysis using machine-learning. You will import and 
format biological data, create an AI model and evaluate its performances. However, this needs a correct Python 
installation to work and using Jupyter Notebook with the correct libraries installed. For the sake of this TD, 
we will use Google Collab Notebooks. However, in the bonus section, you have the instructions to setup your environment
on your local machine.

# 1/ Online Google Collab Notebooks (Fastest and easiest way)
Because it is provided by our lord and saviour Google, you will NEED a Google Account for this to work.  
1. Go to: https://colab.research.google.com/
2. On the pop-up to select Notebook, select the GitHub Tab and enter this link: 
   https://github.com/kchennen/TD_MachineLearning and select the notebook showing (TD_MachineLearning1.ipynb).
3. Download the `healthcare-dataset-stroke-data.csv` dataset available here: 
   [DOWNLOAD](https://www.lbgi.fr/~kchennen/TD_MachineLearning/healthcare-dataset-stroke-data.csv)
4. On the left select the Folder icon and then click the upload file button as indicated in the screenshot and upload 
   the dataset.   
![Upload File](https://i.imgur.com/2WlyUku.png) 
5. You should be able to run notebook and start writing code ! Create a cell and run `print("Hello World")` 
   to check if everything is good !

### **Congratulations** you should now be ready to code for the TD ! 

=> Check out the bonus track at least for the information that it contains ;)  

# Bonus track: The Hard but Worth-It Way ! (As you will be doing it this way in any internship or job)  
It makes everything run on your computer instead of relying on Google's one. 
I will briefly explain each tool to you and how to use them.

1. **Git**  
To Install Git: [Git](https://git-scm.com/downloads) (should already be installed on all Linux)
`Git` is command-line software used in informatics to do code versioning (tracking modifications and updates). 
In any computer science project you WILL be using it. In this TD, we will only use `Git` to download the TD Code from a 
GitHub Repository using the command in a terminal:   
   ```shell
   git clone https://github.com/kchennen/TD_MachineLearning.git
   ```   
   For people that do not want to use Git and could not install it the code is also available as a .zip file 
   [HERE](https://github.com/kchennen/TD_MachineLearning/archive/refs/heads/master.zip)  


2. **Anaconda environment**  
Anaconda is a python distribution and package manager. It is the preferred way for data-scientist to install Python. 
We will use Anaconda to install our **python environment**. An environment is a python installation with a specific set 
of library installed. This way we can ensure that we all have the same package installed with the same version.  
In any Python project, you WILL be using Anaconda environment (or at least Virtual Environment). It is crucial for 
reproducibility, sharing and tracking.  

   **To install our environment**  
   If not already done, install Anaconda from: [Anaconda Download Page](https://www.anaconda.com/products/individual#Downloads)  
   After cloning the Git repository, you will find a file named `environment.yml` containing all information for the 
   Anaconda environment. You can now create the environment using:  
      ```shell
      conda env create -f environment.yml  
      ```
      
   Note: If an error occurs such as `conda is not a valid command` you might need to use the anaconda prompt software 
   for the command. Also, environment are heavy (1.5-2gb here) and can take some time to install.
   You can now activate your environment in your current terminal using:  
   ```shell
   conda activate TD_ML
   ```
   Your command-line should now look like:
   ```shell
   (TD-ML) you@computername:~`
   ```  
   
   For WINDOWS please use Anaconda Prompt terminal or run:
   ```shell
   C:\ProgramData\Anaconda3\Scripts\activate base
   ``` 
   before `conda activate TD_ML` if it doesn't work.


3. **Jupyter Notebooks**  
Jupyter Notebook is the main tool of any data-scientist. It allows you to write and run python code dynamically without 
reloading all the code, data and variables everytime.   
It is structured as blocks of code that you can run and edit independently. In this TD, our main worksheet will be the 
`TD_MachineLearning1.ipynb` Jupyter Notebook.  
You have several option to open Jupyter Notebooks.  
* **The Easy way:** Activate you conda env if not already done. Then run:   
   ```shell
   jupyter-notebook
   ```
  
   Your browser should automatically open a windows on Jupyter or you can simply click the link. Please check if you can 
   open the ipynb file and the folder.  
Note: Don't close the terminal prompt as it would shutdown the Jupyter Server.  
* **The 2nd Way:** Use [VSCode](https://code.visualstudio.com/)  
Install the python extension. VSCode is able to natively open Jupyter Notebook with a great interface and without a 
server. Just select the right python environment, and you're ready to go !  
### **Congratulations** you should now be ready to code for the TD. Simply open the .ipynb file using jupyter-notebook or VSCode !

