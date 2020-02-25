# nonlinear-algebra-code
Code examples for [Nonlinear Algebra](https://math.berkeley.edu/~bernd/math191.html) in Macaulay2.

## Viewing the code

To view the code and the LaTeX in the notebooks properly rendered, go to the following links:

* [Chapter 1: Polynomial Rings (Examples)](https://nbviewer.jupyter.org/github/tyleryzhu/nonlinear-algebra-code/blob/master/Chapter%2001%3A%20Polynomial%20Rings/Ch1-Examples.ipynb?flush_cache=true)
* [Chapter 4: Mapping and Projecting (Exercises)](https://nbviewer.jupyter.org/github/tyleryzhu/nonlinear-algebra-code/blob/master/Chapter%2004%3A%20Mapping%20and%20Projecting/Ch4-Exercises.ipynb?flush_cache=true)

## Getting Started

### Prerequisites

We will be using the Macaulay2 Jupyter Kernel from here: https://github.com/radoslavraynov/Macaulay2-Jupyter-Kernel

You need a recent version of Python and ```pip```. Python 3 is recommended for build installs and necessary for source installs. You can first install Python and pip through the miniconda package manager. First, to download miniconda, go to [the installation site](https://docs.conda.io/en/latest/miniconda.html) and download the installation corresponding to your machine. Then do

```bash
conda install python jupyter pip
```

You will also need an installation of Macaulay2, which can be found [here](http://www2.macaulay2.com/Macaulay2/Downloads/).

Make sure that both ```M2``` and ```M2-binary``` are in ```$PATH```. Check by running

```
$ which M2
/Users/maximsmol/bin/M2
$ which M2-binary
/Users/maximsmol/bin/M2-binary
$ echo $PATH
/Users/maximsmol/M2:/Users/maximsmol/bin/M2-binary:...
```

See [this](https://unix.stackexchange.com/questions/26047/how-to-correctly-add-a-path-to-path) answer if you need to add the binaries to your ```$PATH```.

Finally, to finish the setup, run
```
$ pip install macaulay2-jupyter-kernel
$ python3 -m m2_kernel.install --sys-prefix
```

### Running the code locally

First clone the github repository.
```
$ git clone https://github.com/tyleryzhu/nonlinear-algebra-code.git
$ cd nonlinear-algebra-code
```
To start up a jupyter instance inside this directory, run
```
$ jupyter notebook
```

If you get an error with "Not a directory: 'xdg-settings'", you may need to pass the ```--no-browser``` flag (this is a current bug in Jupyter with Python3.7).

To present a notebook as a presentation, go to View > Cell Toolbar > Slideshow and identify each slide. Then run

```
jupyter nbconvert Chapter\ 1\,\ Polynomial\ Rings.ipynb --to slides --post serve
```

There are also pdfs for your viewing, but those are buggy right now and need to be worked out.

If you have any questions, feel free to open an issue/pull request or email any of the contributors.
