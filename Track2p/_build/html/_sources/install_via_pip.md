# Install via pip

The recommended installation is via `pip` as described on the [home page](https://track2p.github.io/home.html) (and the [GitHub readme](https://github.com/juremaj/track2p)).

The steps are as follows:

First we need to set up a conda environment with python 3.9:

```
conda create --name track2p python=3.9
conda activate track2p
```

Then simply install the track2p package using pip:

```
pip install itk-elastix==0.19.1 --no-deps
pip install track2p
```

Thats it, track2p should be succesfully set up :)
You can simply run it by:

```
python -m track2p
```

This opens a GUI allowing the user to launch the algorithm and visualise the results interactively.

(For instructions on running track2p without the GUI see the 'Run via script' under the 'Usage' section)

Note: For common installation issues see ['Installation > Common issues'](https://track2p.github.io/install_common_issues.html) in documentation.
