# MEETING NOTES

## An introduction to using Jupyter Notebooks

### Before the Workshop - Software Installation
Probably the easiest way to get Jupyter Notebooks up-and-running on most any machine is to download and install [Anaconda (Individual Edition)](https://www.anaconda.com/products/individual). This software package is available for Windows, Mac, and Linux computers.
Once installed, it will allow you to open and run Jupyter Notebooks using your computers graphical interface.

### Workshop notes
**Jupyter file: [20210617_intro_jupyter_notebooks.ipynb](https://github.com/uwlib-python-ig/shared-01/20210617_intro_jupyter_notebooks.ipynb)
- Six participants plus Emilia and Ben
- Some beginners, one participant with experience programming in another language

- Getting started:
   - **Kernel** > **Restart & Clear Output**
- Some features:
   - Creating new cells, the default is a code cell
   - Using **Edit** > **Insert Image** will put the image bitstream into the `.ipynb` so you'll be able to share notebooks without needing to share images separately
   - You can save checkpoints (**File** > **Save and Checkpoint**), this will allow you to return to older versions of your notebooks
- Looking at a "raw" `.ipynb` file
   - Jupyter offers several download options (**File** > **Download as** >)
   - Image files take up most of the space because the bitstreams are large!

### Q&A / comments
- What is the practical upper-limit in terms of the amount of data that can be stored in a notebook?
   - Sometimes running the notebook just takes forever, but the capacity that notebooks can handle seems to be increasing as the software is developed
   - Emilia mentioned that she sets up notebooks so that the data doesn't get stored in the notebook
- Does Jupyter include all Python libraries?
   - They include a lot, but also you can install new packages in the notebook (`! pip install`--the `!` tells Jupyter that you want to use bash)
   - Of course, depending on the package, sometimes they are difficult to install, for example there may be dependencies
   - Pandas, numpy, matplotlib, and much more are included
- If you import libraries would other people also need to do the same importing?
   - Using the in-notebook method above should do the trick (might say "already installed" but shouldn't do any hard)
   - There are also ways to create environments--Emilia showed us the options that she had under **New** > **Notebook**, including specific environments that she created (not sure how setting up an environment works *-BMR*)
   - The Jupyter package has really improved a lot!  

### For the future
- For participants--are there specific tasks that you'd like to perform in a notebook or other Python topics you'd like to learn about? Let [Ben](mailto:ries07@uw.edu) know!
