# 01 Setting up your tools


## Introductions

Ask your partner:

- their formal name
- how they want to be called in class
- what they expect to get from this course
- what useful knowledge or skills they bring to this course


## Syllabus and policies

You can view the syllabus [here](#).


## Set up tools

You need to have the following software set up on your computer:

- the Anaconda distribution of Python 2.7
- up-to-date installations of four packages: `ipython`, `numpy`, `pandas`, and `bokeh`
- a modern, standards-compliant browser (preferably Chrome)

The website [Quantitative Economics](http://quant-econ.net/index.html) has a [short overview](http://quant-econ.net/py/getting_started.html) of how to install Anaconda python and start up the **iPython notebook**. Use the `conda update` command to update each of the packages.

### Install

You can [download Anaconda here](http://continuum.io/downloads). If you use a Windows OS, use `Computer > properties` to find out whether it’s 32-bit or 64-bit, and download the corresponding version of Anaconda.

### Update packages

Start the application named `Terminal` (OS X) or `cmd` (Windows). The resulting window is a **command-line interface**, which we’ll explore later. For now, just use the `conda` command to update your installation. Type `conda update conda` and press `return`. The terminal will inform you that it’s going to download, install, and update a number of packages. Type `y` to proceed. Now repeat this process with the `anaconda` package, by typing `conda update anaconda`. Finally, use the same command to update `ipython`, `numpy`, `pandas`, and `bokeh`.

### Getting to know the command line

```
ls
cd Desktop
ls
touch temp.txt
rm temp.txt
mkdir food
ls
cd food
mkdir fruit
cd fruit
touch apple.txt bananas.txt
cd ..
cd ..
ls food/fruit/
rm food
rmdir food
rm -r food
ipython notebook
```

### IPython Notebook (Jupyter)

Note that the terminal is still running, but appears to be busy doing something. At the same time, your browser created a new window with a listing of files in it. Python is now running, but in the “background”. The new window is an interface where you enter commands. The browser sends the “input” to Python, which does whatever it says, and sends back output. The browser only stores and presents input and output, but does not actually run Python in it. As an example:

    > print “Hello World!”

    Hello World!

    > print “Goodbye!”

    Goodbye!

This makes it great for documenting your work reproducibly. Anyone can download your code and run it on their own Python, and expect to get the same result.

Can the `print` command take numbers? You could look it up, but it might be faster to just try it: 

    > print 55 + 7

    62

    > # Python interprets the output as being an integer
    > print 1/3 

    0

    > 

### Reproducible research


### Literalness

Most programming languages are intolerant of misspellings or misplaced punctuation. In this, they are not that different from human languages. Consider the story of the panda who walks into a pub, has dinner, then pulls out a firearm and shoots a patron in the foot. As he leaves, he calls over his shoulder, “I’m a panda; look it up in the dictionary.” The bartender looks up the definition of panda, which includes “Eats shoots and leaves.” This phrase’s meaning is drastically altered by adding two commas.


## Discussion

Propose a strategy for computing the constant *e* using Python, without relying on a pre-computed value for it.

Ask your partner this questions: **What do we need to know to solve this problem?** Subquestions:

- Observations: What information or concepts do we think are relevant?
- Confusion: What aspect about the problem is confusing?
- Subject: What is the problem about?
- Questions: What information would we like to obtain?

Propose a research strategy:

- What ideas are most relevant to this problem?
- What questions do we need to ask an expert?
- What terms or concepts do we need to look up or read about?
- What techniques or procedures do we need to learn?


## Assignment

Complete [Codecademy tutorials](https://www.codecademy.com/en/tracks/python) up through "Conditionals and Control Flow". (If you've already done this, transfer some random samples of code into IPython notebook and check that it executes without errors in the notebook.)