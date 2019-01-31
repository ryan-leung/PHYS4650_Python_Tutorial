<!-- $theme: default -->

# Python Training Workshop 2019
## An introduction course to Python
### Jan 31, 2019
Ryan Leung 
(yanyan.ryan.leung@gmail.com)

Please go to
<div style="color: #000000; font-family: monospace; font-size: 1em;">
https://tinyurl.com/y6wzrkl5 (introduction)
</div>
<div style="color: #000000; font-family: monospace; font-size: 1em;">
https://tinyurl.com/ybz69nux (hands-on materials)
</div>
<div style="color: #000000; font-family: monospace; font-size: 1em;">
https://tinyurl.com/ybz69nux (Download all notebooks)
</div>

---
## Python: a very fast-growing language
<center>
<img src="assets/images/growth_major_languages.png" alt="drawing" width="600"/>
</center>

---
## A new era of computing

* Varieties of programming languages
* Multi-core CPU and GPU support
* Easily-accessible cloud computing
* Cloud microservices

---
## Python: a versatile language

<center>
<img src="assets/images/Python-logo-notext.svg" alt="drawing" width="200"/>
</center>

* high-level
* object-oriented, and 
* Interpreted

programming language.  

---
## Python: a "High-level language"

* "Low level language": C, Fortran, Basic
* **Level** means the accessiblity to system resources.
* **High Level** : 
  * care less about memory management or proper declaration of variables
  * less abstract than low-level language
  * less time to write and compile
  * relatively slower running time than some low-level language (not always true).

---
## Community of Python users
* Web backend developers
* Data science
* Machine learning

<center>
<img src="assets/images/pythondata_2-map.png" alt="drawing" width="600"/>
</center>
<sub>
Image courtesy of the Python Developers Survey 2017 Results website
</sub>

---
## Python 2 vs Python 3
Results are quoted from https://www.jetbrains.com/research/devecosystem-2018/python/

<center>
<img src="assets/images/python2vspython3.png" alt="drawing" width="600"/>
</center>

---
## Python Usages

<center>
<img src="assets/images/python_packages.png" alt="drawing" width="900"/>
</center>

---
# Installation
* Refer to another guide
* Recommendation:
  * Anaconda
  * Google colab
  
---
## Install packages (with anaconda)
* ```conda search xxxxxx```
* ```conda install xxxxxx```

---
## Install packages (with ``pip``)

``pip`` is a package management system in Python

To search/install packages:
* Search package : ```pip search xxxxxx```
* Install package : ```pip install xxxxxx```
* Upgrade package : ```pip install --upgrade xxxxxx```
* Uninstall package : ```pip uninstall xxxxxx```
* Install wheel package :``` pip install xxxxxx.whl```

---
# Jupyter Notebook
You may want to run a Jupyter notebook when:
* You want to try out a new experiment or analysis with an existing Jupyter notebook from someone.
* You want to develop an algorithm that run on a large software.
* You have only ten minutes to download a data, plot a graph and send the email to your supervisor in a neat format.

![jupyter_logo](assets/images/jupyter_logo.svg)

---
## Open Jupyter in Linux/MacOS
Type 
```bash
jupyter notebook
```
<center>
<img src="assets/images/linux_jupyter.svg" alt="drawing" width="600"/>
</center>


---
## Open Jupyter in Windows
Open your Start menu, goes to ``Anaconda`` Folder,
Click the ``Jupyter Notebook`` shortcut (Recommended). Or start the ``Anaconda Navigator`` and ``Launch``
![windows_jupyter](assets/images/windows_jupyter.svg)

---

## Hand's on Session

The hand's on session requires a working python installations with Jupyter installed. The following links are read-only, they do not run calculations in your computer. 

---

## First Session:
- [Python Syntax](https://nbviewer.jupyter.org/github/ryan-leung/PHYS4650_Python_Tutorial/blob/master/notebooks/01-Python-Syntax.ipynb)
- [Python Data Structures](https://nbviewer.jupyter.org/github/ryan-leung/PHYS4650_Python_Tutorial/blob/master/notebooks/02-Python-Data-Structures.ipynb)
- [Python Numpy Array](https://nbviewer.jupyter.org/github/ryan-leung/PHYS4650_Python_Tutorial/blob/master/notebooks/03-Python-Numpy-Array.ipynb)

---
## Second Session:
- [Introduction to Pandas](https://nbviewer.jupyter.org/github/ryan-leung/PHYS4650_Python_Tutorial/blob/master/notebooks/04-Introduction-to-Pandas.ipynb)
- [Python Functions and Class](https://nbviewer.jupyter.org/github/ryan-leung/PHYS4650_Python_Tutorial/blob/master/notebooks/05-Python-Functions-Class.ipynb)
- [Python Matplotlib](https://nbviewer.jupyter.org/github/ryan-leung/PHYS4650_Python_Tutorial/blob/master/notebook/06-Python-Matplotlib.ipynb)
- [Python plotting with Astropy and AplPy](https://nbviewer.jupyter.org/github/ryan-leung/PHYS4650_Python_Tutorial/blob/master/notebooks/07-Python-Astropy-Aplpy.ipynb)

---
## Online Platforms
Here are some online Python platform that are quite good indeed.

- [c9.io]()
- [repl.it](https://repl.it/)
- [Microsoft Azure Notebooks](https://notebooks.azure.com/)
- [Google Colab](https://colab.research.google.com/)

---
![repl.it](assets/images/repl.it.png)
repl.it

---
![azure-notebook](assets/images/azure-notebook1.png)
Azure Notebook

---
![google-colab](assets/images/google-colab.png)
Google Colab

---
## Online Judge

* [Sphere Online Judge (SPOJ)](http://www.spoj.com/)
* [HackerRank](https://www.hackerrank.com/)
* [CodeAcademy](https://www.codecademy.com/)
* [Aizu Online Judge (AOJ)](http://judge.u-aizu.ac.jp/onlinejudge/index.jsp)

---
## Good Reference Material
- stackoverflow.com

<center>
<img src="https://cdn.sstatic.net/Sites/stackoverflow/company/img/logos/so/so-logo.svg?v=2bb144720a66" alt="drawing" height="100"/>
</center>


- https://github.com/jakevdp/PythonDataScienceHandbook

<center>
<img src="https://raw.githubusercontent.com/jakevdp/PythonDataScienceHandbook/master/notebooks/figures/PDSH-cover.png" alt="drawing" height="300"/>
</center>

- [Book: Python for Astronomers](http://ugastro.berkeley.edu/pydecal/textbook.pdf)

---
## Credits
This tutorial have referenced the following materials:
- [Unidata's online-python-training](https://github.com/Unidata/online-python-training)
- [Anaconda Installation Guide](https://conda.io/docs/user-guide/install/index.html)
- And thanks Sandy Chan and Stephen Ng