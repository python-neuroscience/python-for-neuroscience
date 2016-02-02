.. Metadata
.. --------
:author:      Nicolas P. Rougier
:date:        January 2016
:short-title: Numerical computing
   
              
===================
Numerical computing
===================


Introduction
============

Numpy [Oliphant:2006] is the fundamental package for scientific computing with
Python. It contains among other things:

* a powerful N-dimensional array object
* sophisticated (broadcasting) functions
* tools for integrating C/C++ and Fortran code
* useful linear algebra, Fourier transform, and random number capabilities
* and a lot more...  

Besides its obvious scientific uses, NumPy can also be used as an efficient
multi-dimensional container of generic data. Arbitrary data-types can be
defined and this allows NumPy to seamlessly and speedily integrate with a wide
variety of projects. We are going to explore numpy through a simple example,
implementing the Game of Life.

Game Of Life
============

Numpy is slanted toward scientific computing and we'll consider in this section
the game of life[^1] by John Conway which is one of the earliest example of
cellular automata (see figure below). Those cellular automaton can be
conveniently considered as array of cells that are connected together through
the notion of neighbours. We'll show in the following sections implementation
of this game using pure python and numpy in order to illustrate main
differences with python and numpy.

.. figure:: figures/game-of-life.png

   **Figure 1** Simulation of the game of life.

Exercices
=========

References
==========

.. _[Oliphant:2006] Oliphant, T. E. A guide to numpy. (Trelgol Publishing, 2006).


.. Footnotes
.. ----------------------------------------------------------------------------
          
.. External Links
.. ----------------------------------------------------------------------------

.. _Python:     http://www.python.org
.. _Numpy:      http://www.numpy.org
.. _Scipy:      http://www.scipy.org
.. _Pandas:     http://pandas.pydata.org
.. _Matplotlib: http://matplotlib.org
.. _IPython:    http://ipython.org
.. _Jupyter:    http://jupyter.org
