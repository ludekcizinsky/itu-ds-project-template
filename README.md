## Warning
This repository is still work in progress...

## About 
<!---
Explain in a few lines what this project is about and why should the reader care.

Hint: If you have to write paper or report, you can reuse the intro section.
-->


## Reproducing Results

To reproduce results, two steps are needed:

1) Create virtual environment: **optional**, but recommended so the right
package versions are used

2) Install dependencies via [requirements.txt](requirements.txt)

3) Run the [main function](src/main.py)

These steps are described in detail below.


### Create Virtual Environment

#### Option 1: using `venv`

First, navigate to the folder where you want to
store your virtual environment. (usually one has
a defined folder outside of the project root for
this purpose). Then run the following command (do
not forget the change thee variable in square
brackets):

```
python3 -m venv [name of venv]
```

Now, you can activate the virtual environment
through the command (assuming you are in the
folder where you ran the above command): 

```
source [name of env]/bin/activate
```

You can then deactivate it using:

```
deactivate
```

#### Option 2: using `conda`

You can create a virtual environment within in
`conda` (this assumes you have installed either
[Miniconda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda](https://www.anaconda.com/). 
First, create the new virtual environment with given `python` version through:

```bash
conda create --name [name of venv] python=[python version]
```

Activate the environment 

```
conda activate [name of venv]
```

Check that the `PYTHONPATH` and `PIP` is correctly
udpated by running 

```bash
which python
which pip
```

The output of both should point to a path
including the virtual environments name `[name of venv]` in it.

### Install dependencies and run the code
First, to install the dependencies, run:

```bash
pip install -r requirements.txt
```

Make sure you are at the root of the repository. Finally, to
run the code:

```bash
python cli.py -ALL
``` 
