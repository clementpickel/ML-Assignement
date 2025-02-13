# Machine Learning - Course Assignments

This description will be in each assignment, and it will describe how you install the libraries neccessary to do the assignments.

We assume that you have installed either 'Anaconda' or 'Miniconda' successfully. 

We also assume that you are using VScode. There are other IDE options, but the following description assumes you are using VScode.


## Install libraries with Conda

We need to create a new conda environment to use for all the assignments. Do these following steps to install all the neccessary libraries.

(**For transparency**: The "-y" at the end of all commands - Tell the installation "y" ("yes") beforehand, instead of waiting for the "y/N" promt in the terminal and manually entering "y" when prompted.)

### 1) Open a Conda terminal

First and foremost, open a conda terminal.

If you have installed your conda environment to be availiable in your default OS-terminal, use that if you wish.

### 2) Create a new conda environment

Use the following command to create a new environment:

```Bash
conda create -n ML_course -y
```

Then use this command to switch to the newly created environment:

```Bash
conda activate ML_course
```

We use a seperate environment to not cause any dependency issues with other projects or libraries. Having a seperate environment ensures that we have a 'fresh' installation that will not interfere or be affected by other packages or libraries.


### 3) Install libraries to a conda environment:

We now need to install the libraries into our newly created environment. Run the following command to install packages from the default conda channel:

```Bash
conda install python ipykernel numpy pandas matplotlib -y
```

A brief breakdown of the packages:
* Python - The programing language itself.
* ipykernel - Needed to run python notebooks. (Files ending in ".ipynb")
* numpy - Numeric computation library.
* pandas - Data handling library.
* matplotlib - Data visualization library.

Install 'scikit-learn' using this command since they use the conda-forge download channel:

```Bash
conda install -c conda-forge scikit-learn -y
```

### 4) Done!

You should now be able to use all the libraries neccessary to complete the assignments!

Don't forget to select the correct python-kernel in VScode! (In the top-right corner there is a 'select kernel' button if you do not have a kernel selected)




