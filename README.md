# nonlinear-algebra-code
Code examples for Nonlinear Algebra in Macaulay2

## Getting Started

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

To start up a jupyter instance, run
```
$ jupyter notebook
```

If you get an error with "Not a directory: 'xdg-settings'", you may need to pass the ```--no-browser``` flag (this is a current bug in Jupyter with Python3.7).
