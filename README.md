# pyprobml
Python 3 code for the second edition of my book [Machine learning: a probabilistic perspective](http://people.cs.ubc.ca/~murphyk/MLbook/). This is work in progress, so expect rough edges.

## Notebooks

I have created IPython notebooks for each of the chapters. When you open a notebook, there will be a button at the top that says 'Open in colab'. If you click on this, it will start a virtual machine (VM) instance on Google Cloud Platform (GCP), running [Colab](https://colab.sandbox.google.com/notebooks/welcome.ipynb),  which has all the libraries you will need (e.g., scikit-learn, tensorflow 2, PyTorch) pre-installed. Furthermore, this is free, so all you need is a web browser and an internet connection.

If you select 'GPU' from the 'Runtime' menu at the top of Colab, many examples (especially those that use deep neural networks) will run much faster. The main limitation seems to be the [12GB memory limit](https://github.com/googlecolab/colabtools/issues/253). This should suffice for small experiments. For bigger jobs, you may need to buy cloud credit. Alternatively, you can run these notebooks locally on your desktop in Jupyter, but then you will have to install the packages yourself (see instructions below).

### Foundations
* [Introduction](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/intro/intro.ipynb?flush_cache=true)
* [Linear algebra](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/linalg/linalg.ipynb?flush_cache=true)
* [Calculus](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/calc/calc.ipynb?flush_cache=true)
* [Probability](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/prob/prob.ipynb?flush_cache=true)
* [Information theory](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/info/info.ipynb?flush_cache=true)
* [Bayesian statistics](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/bayes/bayes.ipynb?flush_cache=true)
* [Frequentist statistics](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/freq/freq.ipynb?flush_cache=true)
* [Statistical models: discriminative](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/statmod-discrim/statmod-discrim.ipynb?flush_cache=true)
* [Statistical models: generative](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/statmod-gen/statmod-gen.ipynb?flush_cache=true)
* [Statistical models: structured](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/statmod-struct/statmod-struct.ipynb?flush_cache=true)

### Algorithms
* [Optimization: continuous problems](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/opt-cts/opt-cts.ipynb?flush_cache=true)
* [Optimization: discrete and blackbox problems](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/opt-discrete/opt-discrete.ipynb?flush_cache=true)
* [Belief propagation](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/bp/bp.ipynb?flush_cache=true)
* [Variational methods](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/vi/vi.ipynb?flush_cache=true)   
* [Monte Carlo methods](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/mc/mc.ipynb?flush_cache=true)

### Models
* [Sparse models](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/sparse/sparse.ipynb?flush_cache=true)
* [Deep neural networks](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/dnn/dnn.ipynb?flush_cache=true)
* [Gaussian processes](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/gp/gp.ipynb?flush_cache=true)
* [Other kernel methods](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/kernel/kernel.ipynb?flush_cache=true)
* [Other Bayesian non-parametric models](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/npbayes/npbayes.ipynb?flush_cache=true)
* [Graphical models](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/pgm/pgm.ipynb?flush_cache=true)
* [Latent factor models](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/lfm/lfm.ipynb?flush_cache=true)
* [Other deep generative models](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/genmo/genmo.ipynb?flush_cache=true)
* [Models for sequences](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/seq/seq.ipynb?flush_cache=true)
* [Models for graphs](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/graphs/graphs.ipynb?flush_cache=true)
* [Models for reinforcement learning](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/rl/rl.ipynb?flush_cache=true)
* [Causal models](https://nbviewer.jupyter.org/github/probml/pyprobml/blob/master/notebooks/causal/causal.ipynb?flush_cache=true)

## Scripts

Many of the figures in the book are generated by these  [scripts](scripts). To execute a script, cd (change directory) to the scripts folder, and then type 'python foo.py'. You can also run each script from inside a Python IDE (like Spyder).
Many of the scripts create plots, which are saved to ../figures.


### Installation

To run the scripts, we assume you have installed numpy, scipy, matplotlib, seaborn, pandas, scikit-learn, etc.
(All of these are bundled with [anaconda](https://www.anaconda.com/distribution/).)
Some scripts rely on additional libraries, such as [Tensorflow 2.0](https://www.tensorflow.org/) and [JAX](https://github.com/google/jax). Scripts that need these libraries have filenames that end in tf and jax respectively.
If you have problems running these, open up one of the notebooks above in Google Colab - which will have the various packages already installed - and then import the script.

