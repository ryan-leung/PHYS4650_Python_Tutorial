# Installing Anaconda on MacOS

## Download Anaconda

### From Anaconda site
1. Download Anaconda installer for MacOS from here: [https://www.anaconda.com/download/](https://www.anaconda.com/download/)
2. Choose ``Python 2.7`` or ``Python 3.6``, read
[python2 vs python3](./python2-vs-python3.md)

### From Anaconda repository
1. Download Anaconda installer for MacOS from here: https://repo.continuum.io/archive/ from the browser.
2. There are two type ``.sh`` and ``.pkg``, ``.sh`` requires you to use the Terminal.app while ``.pkg`` install with double-click.
3. Here I will show you how to install via Terminal.app

## Installing Anaconda via Terminal.app
1. Open up a terminal.
2. ``cd`` to your instaler folder, usually ``~/Downloads/``.
3. Type ``sh ./AnacondaXXXXXXXX.sh``, where ``AnacondaXXXXXXXX.sh`` refers to the downloaded file name.
4. Follow the instructions on the screen. Accept the
defaults if you are not sure what to do :stuck_out_tongue:.
5. Installation will be finished within 5 minutes.
6. The following line will be appeared:
``Do you wish the installer to prepend the AnacondaX install location to PATH in your /Users/XXX/.bash_profile ? [yes|no]``
7. If you use ``bash``, you can type ``yes`` for easy installation. Read the next session about ``PATH variable``
8. Everything is done. Refresh your bash terminal by ``source ~/.bash_profile`` 

## Anaconda ``PATH`` variable
The Anaconda will **NOT** append the ``PATH`` variable during Linux installation. To qurantee your installation is successful, you need to check your rcfile for Bash, i.e. the ``.bash_profile`` stored under the Home directory of MacOS. To read the ``.bash_profile``:
1. Type ``cat ~/.bash_profile`` in your terminal.
2. If you have the following lines at the end, it means the installation is ok.
```
# added by Anaconda2 installer
export PATH="/Users/XXXXX/anacondaX/bin:$PATH"
```
3. If you doesn't got this line, first check the Anaconda installation location (usually /Users/XXXXX/anacondaX/) and add the following line (Replace /Users/XXXXX/anacondaX/ with your installation location) to ``~/.bash_profile`` using a text editor:
```
export PATH="/Users/XXXXX/anacondaX/bin:$PATH"
```
4. If you have no idea what is a text editor, open a terminal,
type ``echo "export PATH="/Users/XXXXX/anacondaX/bin:$PATH"" >> ~/.bash_profile`` and enter, of course you need to replace your installation folder here.

## Successful Anaconda installation
1. Run ``source ~/.bash_profile`` in the terminal.
2. Type ``python`` in the terminal.
3. Similar strings will be appeared: :heavy_check_mark:
```
Python 2.7.14 |Anaconda custom (64-bit)| (default, Oct 16 2017, 17:29:19) 
[GCC 7.2.0] on linux2
Type "help", "copyright", "credits" or "license" for more information. 
```
4. If the following similar strings appeared, redo the previous session or run ``source ~/.bash_profile`` in the terminal. :heavy_multiplication_x:
```
Python 2.7.14 (default, Jan  5 2018, 10:41:29) 
[GCC 7.2.1 20171224] on linux2
Type "help", "copyright", "credits" or "license" for more information.
```

## Updating conda

1. Open a terminal.
2. Run ``conda update anaconda``.

## Uninstalling conda

1. Open a terminal.
2. Check the Anaconda installation path.
3. Usually ``~/anacondaX/``
4. Run ``rm -fr ~/anacondaX/``
5. Open your ``~/.bash_profile``
6. Find and remove the line ``export PATH="/Users/XXXXX/anacondaX/bin:$PATH"``
7. Run ``source ~/.bash_profile``