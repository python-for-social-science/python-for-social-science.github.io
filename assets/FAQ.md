# Frequently Asked Question

## Python is used for many essential operations on Linux and OS X.  Does Anaconda use its own install of Python or the system's?

Anaconda comes with its own separate version of Python. The version of Python that Anaconda installs is independent of any versions of Python you might have on your computer, or any future versions of Python you decide to install afterwards. 

The same can be said for all of the apps that come with Anaconda: Users can download and install a bunch of programming software without worrying about compatibility. You don't need to be concerned about your version of Rstudio or JupyterLab crashing because you had the wrong version of some obscure Python library installed on your computer.

## What is a package manager?

A package manager is a tool that automates downloading, installing, and updating programs. When your phone or computer notifies you that updates are available, that's the package manager. 

Python has its own package management system called `pip`. There are thousands upon thousands of specialized tools, programs, functions, libraries for any job you can imagine. `pip` exists to help you find and install these packages to extend Python's capabilities. 

Anaconda has its own package management system too, called `conda`. With it, users can install entire programming software stacks such as R, Python, Django, PostgreSQL, etc...

## What if I need a package that does not come with the Anaconda distribution?

_Unsure about this question, Zach. Are we talking python packages? I think you mean what if theres a package I need (say `numpy`) and anaconda doesn't come with it right away?_ 

If you need a package that didn't come with Anaconda, use `pip`! For example, you may need to install `numpy`, which handles more complex math functions, yourself. To do that, you would write 

```
pip install numpy
```

and run the command. Now the `numpy` package is available for you to load into your code.

## What is a virtual environment and why would I use one?

A virtual environment is a way to freeze the versions of all the software and software packages your coding project needs to run. If you wrote a project in Python five years ago and tried to run it today, it would probably not work because you used older versions of packages. Virtual environments provide a solution to this problem: You specify the version numbers of Python itself, your packages and extensions, third-party libraries, etc. This ensures that code which works at one point in time will keep working if packages change or stop being compatible at some point in the future.

## Why does Jupyter open in a browser tab instead of its own program?

Compatibility! Jupyter opens in a browser because web user interfaces are really standardized. You can deliver the same product whether on a Mac, Windows, or Linux machine. Secondly, not needing to write a new graphical user interface, and piggybacking on HTML and CSS saves the Jupyter developers _a lot_ of time and money.

## How do I change the default location of a new Jupyter notebook opened in Anaconda Navigator?

Any time you create a new notebook in JupyterLab, an `untitled.ipynb` file is generated and saved in whatever current folder/path you are inside of (You can check this on the files and folders sidebar (`Ctrl+Shift+F`)).

keep this in mind for your assignments and projects because the location of your Notebook file determines the relative path for loading data from other folders on your computer.

In case you are using JupyterNotebook, that program always opens in your computer's home folder. The link below shows you how to change your default startup folder through anaconda.
https://www.planetofbits.com/python/change-jupyter-notebook-startup-folder-anaconda/

## Does JupyterLab offer code autocompletion?

Yes it does. Press tab while typing a python function and JupyterLab will display a drop-down list of possible functions that match what you have written.

## When I execute code from a cell, it does not use output created when I executed via the Run dropdown menu?  Why?  Is that behavior going to cause problems?

## If I execute multiple lines of code at once, the console only displays the final line.  For example, the lines "df.shape; df.head(); df.iloc[100:105] will only show rows 100-105 of df.  How do I make JupyterLab display the output of all lines?

## Does JupyterLab have a spellchecker for Markdown cells?

## Sometimes code takes longer to execute than I want.  How do I make it stop?
The easy answer is the stop button or Kernel->Interrupt Kernel.  This can be finicky and not feel like it's working.  When that happens, press the stop button repeatedly over and over in quick succession.  If that does not work, see this [StackOverflow thread with other ideas.](https://stackoverflow.com/questions/42750753/how-to-stop-the-running-cell-if-interrupt-kernel-does-not-work-in-jupyter-notebo)  Unfortunately, this problem has been known for ten years but is not resolved.
