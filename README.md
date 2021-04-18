### UNC_RAx_Tutorial
==============================
#### Using Generalised Read-Across (GenRA) to make predictions of toxicity

This tutorial introduces read-across, a data gap filling technique that is used within analogue and category approaches. Read-across is where information on a property for a source (data rich) substance is used to predict the same property for a target (data poor) substance. Read-across is typically an expert-driven subjective assessment but there have been efforts to develop objective systematic approaches to read-across. One example is Generalised Read-Across (GenRA) which relies on calculating a similarity weighted activity of nearest neighbours (source analogues). In this tutorial, the goal is for participants to develop a sound conceptual understanding on what read-across is and to obtain some hands-on experience of using GenRA to predict the median lethal dose (LD50) of acute oral rat toxicity studies for substances lacking that information. 

#### Prerequisites
Participants will be expected to be reasonably comfortable using Python with some prior exposure to NumPy, Pandas, Scikit-learn and RDKit. It would help if you knew:
- programming fundamentals and the basics of the Python programming language (e.g. variables, for loops)
- some experience with working with DataFrames within Pandas
- some prior experience of using Jupyter Notebooks

If you are going to code along, suggest you use the Anaconda distribution of Python 3.

#### Getting set up computationally

The first option and the easiest option is to use Binder. This will spin up the necessary computational environment for you to write and execute Python code from your browser. Another option is to pull the Docker image with genra-py preinstalled using `docker pull patlewig/genra-py` and following the instructions provided in the dockerhub description.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/patlewig/UNC_Rax/HEAD)

Alternatively:

1. Clone the repository
You can do this by executing the following in your terminal:

`git clone https://github.com/patlewig/UNC_RAx_Tutorial`

If you don't feel comfortable using git, you can always download the zip file of the repository at the top of the main page of the repository.

2. Download and install Anaconda

3. Create your conda environment for this session
Navigate to the relevant directory UNC_RAx_Tutorial and install the required packages in a new conda environment:

`conda env create -f environment.yml`

This will create a new environment called UNC_RAx_Tutorial. To activate the environment execute:

`conda activate UNC_RAx_Tutorial`

GenRA (genra-py) will need to be installed in this activated environment with:
`pip install -i https://test.pypi.org/simple/ genra`

4. Open your Jupyter Notebook
In the terminal, execute `jupyter notebook`.
Then open the notebook `01-Student-GenRA.ipynb` and we can start coding!










