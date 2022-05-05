## What are we doing? 
Recently the topic of [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code) came up, which are a neat (if hacky) way to do some cool stuff in your terminal - or in Jupyter Notebooks. One of the cooler things you can do with them is to change the styling of text. Using the right escape codes you can make your text bold, italic, or underlined - as well as making the text and the background whatever color you want. 

To make a long story short, we wanted to see if we could take an image and convert it to a bunch of colored ▄ characters that we could print to stdout. This can be dispalyed in a jupyter notebook or your terminal. 

## Some Remarks
- The code in this notebook does everything it's supposed to, but it'll screw up if you run the notebook in VS Code instead of launching jupyter notebook and running it there. This is because VS Code sets the background color in some way that the ANSI escape codes don't overrule.
- I've included a conda environment file. You can build the environment with `conda env create -f /path/to/jupy.yaml`, and then you can activate it with `conda activate jupy`
    - if you don't have conda just make sure you install pillow and you're probably fine. This doesn't use many libraries so I doubt you'll run into issues.
- If you try copy/pasting the code into your terminal you might run into issues. Windows recognizes ANSI escape codes and it tries to do some stuff with them (?). IDK. 