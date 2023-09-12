> library(reticulate)
> py_run_string("from pdf2docx import parse")
> py_run_string("from pdf2docx import parse")


Error in py_run_string_impl(code, local, convert) : 
  ModuleNotFoundError: No module named 'pdf2docx'
Run `reticulate::py_last_error()` for details.


User was not able to download python packages from R.

We first installed reticulate

https://rstudio.github.io/reticulate/reference/install_python.html


---

Would you like to create a default python environment for the reticulate package? (Yes/no/cancel) yes
Error in stop_no_virtualenv_starter(version = version, python = python) : 
  Suitable Python installation for creating a venv not found.
  Requested Python: /usr/local/bin/python3.9
Please install Python with one of following methods:
- https://github.com/rstudio/python-builds/
- reticulate::install_python(version = '<version>')
> py_run_string("from pdf2docx import parse")
Would you like to create a default python environment for the reticulate package? (Yes/no/cancel) no
Error: Python shared library not found, Python bindings not loaded.
Please create a default virtual environment with `reticulate::virtualenv_create('r-reticulate')`.
> library(reticulate)
> py_run_string("from pdf2docx import parse")
Would you like to create a default python environment for the reticulate package? (Yes/no/cancel) yes
Error in stop_no_virtualenv_starter(version = version, python = python) : 
  Suitable Python installation for creating a venv not found.
  Requested Python: /usr/local/bin/python3.9
Please install Python with one of following methods:
- https://github.com/rstudio/python-builds/
- reticulate::install_python(version = '<version>')
> py_install("pdf2docx", pip = TRUE) 
Error in stop_no_virtualenv_starter(version = version, python = python) : 
  Suitable Python installation for creating a venv not found.
  Requested Python: /usr/local/bin/python3.9
Please install Python with one of following methods:
- https://github.com/rstudio/python-builds/
- reticulate::install_python(version = '<version>')
> install_python(version = "3.9:latest", list = FALSE, force = FALSE)
trying URL 'https://github.com/pyenv/pyenv-installer/raw/master/bin/pyenv-installer'
Content type 'text/plain; charset=utf-8' length 2827 bytes
==================================================
downloaded 2827 bytes

Installing pyenv ...
Cloning into '/home/ashish.j189/.local/share/r-reticulate/pyenv'...
remote: Enumerating objects: 1162, done.
remote: Counting objects: 100% (1162/1162), done.
remote: Compressing objects: 100% (668/668), done.
remote: Total 1162 (delta 673), reused 634 (delta 361), pack-reused 0
Receiving objects: 100% (1162/1162), 578.73 KiB | 3.62 MiB/s, done.
Resolving deltas: 100% (673/673), done.
Cloning into '/home/ashish.j189/.local/share/r-reticulate/pyenv/plugins/pyenv-doctor'...
remote: Enumerating objects: 11, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 11 (delta 1), reused 5 (delta 0), pack-reused 0
Receiving objects: 100% (11/11), 38.72 KiB | 1.84 MiB/s, done.
Resolving deltas: 100% (1/1), done.
Cloning into '/home/ashish.j189/.local/share/r-reticulate/pyenv/plugins/pyenv-update'...
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 10 (delta 1), reused 5 (delta 0), pack-reused 0
Receiving objects: 100% (10/10), done.
Resolving deltas: 100% (1/1), done.
Cloning into '/home/ashish.j189/.local/share/r-reticulate/pyenv/plugins/pyenv-virtualenv'...
remote: Enumerating objects: 63, done.
remote: Counting objects: 100% (63/63), done.
remote: Compressing objects: 100% (56/56), done.
remote: Total 63 (delta 11), reused 29 (delta 0), pack-reused 0
Receiving objects: 100% (63/63), 40.54 KiB | 2.03 MiB/s, done.
Resolving deltas: 100% (11/11), done.

WARNING: seems you still have not added 'pyenv' to the load path.

# Load pyenv automatically by appending
# the following to 
~/.bash_profile if it exists, otherwise ~/.profile (for login shells)
and ~/.bashrc (for interactive shells) :

export PYENV_ROOT="$HOME/.pyenv"
command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"

# Restart your shell for the changes to take effect.

# Load pyenv-virtualenv automatically by adding
# the following to ~/.bashrc:

eval "$(pyenv virtualenv-init -)"

Done! pyenv has been installed to '/home/ashish.j189/.local/share/r-reticulate/pyenv/bin/pyenv'.
Cloning into '/home/ashish.j189/.pyenv/plugins/pyenv-update'...
remote: Enumerating objects: 81, done.
remote: Counting objects: 100% (22/22), done.
remote: Compressing objects: 100% (14/14), done.
remote: Total 81 (delta 8), reused 11 (delta 3), pack-reused 59
Receiving objects: 100% (81/81), 15.60 KiB | 7.80 MiB/s, done.
Resolving deltas: 100% (29/29), done.
+ /home/ashish.j189/.local/share/r-reticulate/pyenv/bin/pyenv update
+ /home/ashish.j189/.local/share/r-reticulate/pyenv/bin/pyenv install --skip-existing 3.9.18
Downloading Python-3.9.18.tar.xz...
-> https://www.python.org/ftp/python/3.9.18/Python-3.9.18.tar.xz
Installing Python-3.9.18...
Traceback (most recent call last):
  File "<string>", line 1, in <module>
  File "/home/ashish.j189/.pyenv/versions/3.9.18/lib/python3.9/sqlite3/__init__.py", line 57, in <module>
    from sqlite3.dbapi2 import *
  File "/home/ashish.j189/.pyenv/versions/3.9.18/lib/python3.9/sqlite3/dbapi2.py", line 27, in <module>
    from _sqlite3 import *
ModuleNotFoundError: No module named '_sqlite3'
WARNING: The Python sqlite3 extension was not compiled. Missing the SQLite3 lib?
Installed Python-3.9.18 to /home/ashish.j189/.pyenv/versions/3.9.18
[1] "/home/ashish.j189/.pyenv/versions/3.9.18/bin/python3.9"
> py_run_string("from pdf2docx import parse")
Would you like to create a default python environment for the reticulate package? (Yes/no/cancel) yes
Using Python: /home/ashish.j189/.pyenv/versions/3.9.18/bin/python3.9
Creating virtual environment 'r-reticulate' ... 
+ /home/ashish.j189/.pyenv/versions/3.9.18/bin/python3.9 -m venv /home/ashish.j189/.virtualenvs/r-reticulate
Done!
Installing packages: pip, wheel, setuptools
+ /home/ashish.j189/.virtualenvs/r-reticulate/bin/python -m pip install --upgrade pip wheel setuptools
Requirement already satisfied: pip in ./.virtualenvs/r-reticulate/lib/python3.9/site-packages (23.0.1)
Collecting pip
  Downloading pip-23.2.1-py3-none-any.whl (2.1 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2.1/2.1 MB 3.5 MB/s eta 0:00:00
Collecting wheel
  Downloading wheel-0.41.2-py3-none-any.whl (64 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 64.8/64.8 kB 13.1 MB/s eta 0:00:00
Requirement already satisfied: setuptools in ./.virtualenvs/r-reticulate/lib/python3.9/site-packages (58.1.0)
Collecting setuptools
  Downloading setuptools-68.2.1-py3-none-any.whl (807 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 807.9/807.9 kB 2.8 MB/s eta 0:00:00
Installing collected packages: wheel, setuptools, pip
  Attempting uninstall: setuptools
    Found existing installation: setuptools 58.1.0
    Uninstalling setuptools-58.1.0:
      Successfully uninstalled setuptools-58.1.0
  Attempting uninstall: pip
    Found existing installation: pip 23.0.1
    Uninstalling pip-23.0.1:
      Successfully uninstalled pip-23.0.1
Successfully installed pip-23.2.1 setuptools-68.2.1 wheel-0.41.2
Installing packages: numpy
+ /home/ashish.j189/.virtualenvs/r-reticulate/bin/python -m pip install --upgrade --no-user numpy
Collecting numpy
  Obtaining dependency information for numpy from https://files.pythonhosted.org/packages/69/1f/c95b1108a9972a52d7b1b63ed8ca70466b59b8c1811bd121f1e667cc45d8/numpy-1.25.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata
  Downloading numpy-1.25.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata (5.6 kB)
Downloading numpy-1.25.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (18.3 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 18.3/18.3 MB 4.4 MB/s eta 0:00:00
Installing collected packages: numpy
Successfully installed numpy-1.25.2
Virtual environment 'r-reticulate' successfully created.
Error in py_run_string_impl(code, local, convert) : 
  ModuleNotFoundError: No module named 'pdf2docx'
Run `reticulate::py_last_error()` for details.
> py_install("pdf2docx", pip = TRUE) 
Using virtual environment '/home/ashish.j189/.virtualenvs/r-reticulate' ...
+ /home/ashish.j189/.virtualenvs/r-reticulate/bin/python -m pip install --upgrade --no-user pdf2docx
Collecting pdf2docx
  Using cached pdf2docx-0.5.6-py3-none-any.whl (148 kB)
Collecting PyMuPDF>=1.19.0 (from pdf2docx)
  Obtaining dependency information for PyMuPDF>=1.19.0 from https://files.pythonhosted.org/packages/da/4f/a2b9479145cca44d30706ac3612c6d8c6aecae962b85c833fbe0012b4050/PyMuPDF-1.23.3-cp39-none-manylinux2014_x86_64.whl.metadata
  Downloading PyMuPDF-1.23.3-cp39-none-manylinux2014_x86_64.whl.metadata (3.4 kB)
Collecting python-docx>=0.8.10 (from pdf2docx)
  Using cached python-docx-0.8.11.tar.gz (5.6 MB)
  Preparing metadata (setup.py) ... done
Collecting fonttools>=4.24.0 (from pdf2docx)
  Obtaining dependency information for fonttools>=4.24.0 from https://files.pythonhosted.org/packages/49/50/2e31753c088d364756daa5bed0dab6a5928ebfd6e6d26f975c8b6d6f754a/fonttools-4.42.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata
  Downloading fonttools-4.42.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata (150 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 151.0/151.0 kB 1.0 MB/s eta 0:00:00
Requirement already satisfied: numpy>=1.17.2 in ./.virtualenvs/r-reticulate/lib/python3.9/site-packages (from pdf2docx) (1.25.2)
Collecting opencv-python>=4.5 (from pdf2docx)
  Obtaining dependency information for opencv-python>=4.5 from https://files.pythonhosted.org/packages/f5/d0/2e455d894ec0d6527e662ad55e70c04f421ad83a6fd0a54c3dd73c411282/opencv_python-4.8.0.76-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata
  Downloading opencv_python-4.8.0.76-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata (19 kB)
Collecting fire>=0.3.0 (from pdf2docx)
  Using cached fire-0.5.0.tar.gz (88 kB)
  Preparing metadata (setup.py) ... done
Collecting six (from fire>=0.3.0->pdf2docx)
  Using cached six-1.16.0-py2.py3-none-any.whl (11 kB)
Collecting termcolor (from fire>=0.3.0->pdf2docx)
  Using cached termcolor-2.3.0-py3-none-any.whl (6.9 kB)
Collecting PyMuPDFb==1.23.3 (from PyMuPDF>=1.19.0->pdf2docx)
  Obtaining dependency information for PyMuPDFb==1.23.3 from https://files.pythonhosted.org/packages/34/cf/bb6a3bad0ffdea1fb9fcae53de6c1b9187746c32e17377ff8f36b9d98ee4/PyMuPDFb-1.23.3-py3-none-manylinux2014_x86_64.manylinux_2_17_x86_64.whl.metadata
  Downloading PyMuPDFb-1.23.3-py3-none-manylinux2014_x86_64.manylinux_2_17_x86_64.whl.metadata (1.3 kB)
Collecting lxml>=2.3.2 (from python-docx>=0.8.10->pdf2docx)
  Obtaining dependency information for lxml>=2.3.2 from https://files.pythonhosted.org/packages/cc/b9/d822b2fc9b9406cff3ec6be03d69adb0e44fcad09608489ea4acaf2443bb/lxml-4.9.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl.metadata
  Downloading lxml-4.9.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl.metadata (3.8 kB)
Downloading fonttools-4.42.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (4.5 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.5/4.5 MB 3.6 MB/s eta 0:00:00
Using cached opencv_python-4.8.0.76-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (61.7 MB)
Downloading PyMuPDF-1.23.3-cp39-none-manylinux2014_x86_64.whl (4.3 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 4.3/4.3 MB 4.0 MB/s eta 0:00:00
Downloading PyMuPDFb-1.23.3-py3-none-manylinux2014_x86_64.manylinux_2_17_x86_64.whl (30.6 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 30.6/30.6 MB 4.1 MB/s eta 0:00:00
Downloading lxml-4.9.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl (7.1 MB)
   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 7.1/7.1 MB 4.4 MB/s eta 0:00:00
Building wheels for collected packages: fire, python-docx
  Building wheel for fire (setup.py) ... done
  Created wheel for fire: filename=fire-0.5.0-py2.py3-none-any.whl size=116934 sha256=17131079e63a739d2226488a749e67a5d9d447b03c4b60a30d9de22570a7832c
  Stored in directory: /home/ashish.j189/.cache/pip/wheels/f7/f1/89/b9ea2bf8f80ec027a88fef1d354b3816b4d3d29530988972f6
  Building wheel for python-docx (setup.py) ... done
  Created wheel for python-docx: filename=python_docx-0.8.11-py3-none-any.whl size=184487 sha256=b72a95e03a0cdc07e9a2d8fa99428ab08134f97ad2da6fd5049e0d2fb6bfecde
  Stored in directory: /home/ashish.j189/.cache/pip/wheels/83/8b/7c/09ae60c42c7ba4ed2dddaf2b8b9186cb105255856d6ed3dba5
Successfully built fire python-docx
Installing collected packages: termcolor, six, PyMuPDFb, opencv-python, lxml, fonttools, python-docx, PyMuPDF, fire, pdf2docx
Successfully installed PyMuPDF-1.23.3 PyMuPDFb-1.23.3 fire-0.5.0 fonttools-4.42.1 lxml-4.9.3 opencv-python-4.8.0.76 pdf2docx-0.5.6 python-docx-0.8.11 six-1.16.0 termcolor-2.3.0
> py_run_string("from pdf2docx import parse")
> 
Save workspace image? [y/n/c]: n
[GENINVO\ashish.j189@a-qqhw42j48nfs ~]$ ls /home/
ashish.j189  chanchal.b253  damanjeet.s11
[GENINVO\ashish.j189@a-qqhw42j48nfs ~]$ ^C
[GENINVO\ashish.j189@a-qqhw42j48nfs ~]$ 
