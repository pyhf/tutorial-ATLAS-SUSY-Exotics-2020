# [ATLAS Exotics + SUSY Workshop 2020 `pyhf` Tutorial](https://indico.cern.ch/event/898965/sessions/355806/)

## Welcome!

<p align="center">
<a href="https://github.com/scikit-hep/pyhf"><img src="https://raw.githubusercontent.com/scikit-hep/pyhf/master/docs/_static/img/pyhf-logo-small.png"></a>
</p>

Welcome to the `pyhf` tutorial given at the [ATLAS Exotics + SUSY Workshop 2020](https://indico.cern.ch/event/898965/)!
We'll first point you towards our documentation website ([scikit-hep.org/pyhf/](https://scikit-hep.org/pyhf/)) and recommend that you visit it for much more detailed explanations and examples.
Let's dive right in.

We won't review the full pedagogy of `HistFactory`, so instead we'll point you to
the [`pyhf` talk at SciPy 2020](https://github.com/matthewfeickert/talk-SciPy-2020).

<!-- http://www.get-youtube-thumbnail.com/ -->
[![SciPy 2020 talk YouTube](http://i3.ytimg.com/vi/FrH9s3eB6fU/maxresdefault.jpg)](https://youtu.be/FrH9s3eB6fU)

Instead, let's move to looking at the `pyhf` API right away.

## Installation

If you haven't already, make a new Python 3 virtual environment and then install `pyhf` from either [PyPI](https://pypi.org/project/pyhf/) with `pip`

```
(pyhf-tutorial) $ python -m pip install pyhf
```

 or [Conda-forge](https://anaconda.org/conda-forge/pyhf)

```
(pyhf-tutorial) $ conda config --add channels conda-forge
(pyhf-tutorial) $ conda install pyhf
```

### Installation Extras

If you're installing from PyPI, you can also install with some of the "extras" that will be useful for doing typical HEP analysis workflows with `pyhf`.

````{tabbed} Read/Write XML+ROOT
```
(pyhf-tutorial) $ python -m pip install pyhf[xmlio]
```

The 'xmlio' extra additionally installs [`uproot`](https://github.com/scikit-hep/uproot) to read `ROOT` files.
````

````{tabbed} Use PyTorch and Tensorflow
```
(pyhf-tutorial) $ python -m pip install pyhf[torch,tensorflow]
```

The 'torch' extra installs [`pytorch`](https://pytorch.org/) and the 'tensorflow' extra installs [`tensorflow`](https://www.tensorflow.org/).
````

See our [installation docs](https://scikit-hep.org/pyhf/installation.html) for more information about installation options.

### Dependencies for this tutorial

To get all the dependencies needed for this tutorial you can just install from the included `requirements.txt` in the top level `binder/` directory of [the source repository](https://github.com/pyhf/tutorial-ATLAS-SUSY-Exotics-2020)

```
(pyhf-tutorial) $ python -m pip install -r binder/requirements.txt
```
