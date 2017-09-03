=======
PyTURNS
=======
If we had to rewrite OpenTURNS, how would we do it the Python way?

Why?
====
- Consistency, avoid duplication with the scientific Python ecosystem (numpy.array etc)
- Focus on the core of OpenTURNS

Ideas
=====
- Use numpy.array as samples
- Use native Python functions (can we drop the input/dimension properties, gradients ?)
- Drop optimization algorithm wrappers in favor of scipy.optimize (also drop EGO in favor of skopt.gp_minimize)
- Drop bayesian (pymc)
- Drop kriging (sklearn)
- Contribute scipy.stats distributions
