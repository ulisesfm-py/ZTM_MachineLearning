#Installing Miniconda on Linux

1. [Download Miniconda installer for Linux](https://docs.conda.io/en/latest/miniconda.html#linux-installers)
2. [Verify your installer hashes](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html#hash-verification) 
3. In your terminal run:

'''bash
Miniconda3-latest-Linux-x86_64.sh
'''

4. Follow the prompts on the installer screens.
5. Verify that conda is installed and running by typing:

'''bash
conda --version
'''

6. Update conda to the current version.

'''bash
conda update conda
'''

#Managing environments

Conda allows you to create separate environments containing files, packages and their dependencies.

1. Create a new environment and install a package in it. We will call the environment 'sample_project' and install a few packages like jupyter and pandas:

'''bash
conda create --name sample_project jupyter pandas scikit-learn numpy
'''

2. To see the current environments write:

'''bash
conda env list
'''

or

'''bash
conda info --envs
'''

3. To activate an enviroment write this, changing the path with the actual path shown in the env list:

'''bash
conda activate /home..../sample_project 
'''

# Managing packages

1. Check if you already have installed a package:

'''bash
conda search beautifulsoup4
'''

2. If it is not install you can install it doing:

'''bash 
conda install beautifulsoup4
'''

3. Check the installed programs in the environment:

'''bash
conda list
'''