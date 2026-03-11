# Martin Esteban Yunge Rivas - MYR2003 - iit414w 11/03/2026
Repository for AI Workshop

## System information
OS: NobaraOS (Fedora-based distribution)
Kernel version: 6.19.5-200.nobara.fc43.x86_64
Python version: Python 3.14.2
Pip version: pip 25.1.1

## Setup instructions
(Python and pip must be installed and on the right versions)
Open up a terminal on the root folder of the Repository then run the next commands:
- python -m venv venv # This will create the python enviroment
- source venv/bin/activate # To activate the enviroment and use it on Linux/MacOS
- .\venv\Scripts\activate #  To activate the enviroment and use it on Windows
Now open up the "requirements.txt" and install all dependencies on the specific versions, example:
- pip install numpy==2.4.2

## How to run
Now that the enviroment is installed you will need VScode with the jupyter notebook extension and python extension installes.
First of all open the setup_check.ipynb file, then at the top right corner of the file you have a "select kernel" options, select it and then select the virtual enviroment.
Now run it, you can run it cell by cell or using the run all function.

Now the same goes for the second file data_check.ipynb, open the file, select the kernel, and run the file.

## Problems encountered
- Problem install sklearn. Solution I read the output and found that the solution was installing it with another name "scikit-learn"
- Problem showing matplotlib version on setup_check. Solution importing matplotlib and showing the version, matplotlib.pyplot the one we are using dosen't have the attribute version
- VScode not detecting the virtual environment. Solution manully adding the environment.
- There was no necessitie for the following lines:
    - cache_path = os.path.join(os.path.dirname(os.getcwd()), 'data', 'fastf1_cache')
    - cache_path = os.path.abspath(cache_path)
The send the cache folder outside the root folder of the project. Solution this next line:
    - cache_path = os.path.join(os.getcwd(), 'data', 'fastf1_cache')
This is the version well written of the code.

## Expected outputs
