# XBUS-519: Machine Learning Creativity

This repository contains some example code to get you started with music composition and image generation using Python. However, because of the extensive requirements for setup and issues with different operating systems - most the of the workshops will focus on tools that can be accessed on the web. After the class, please feel free to use these resources and if you have any questions, open a GitHub issue.

## Workshop 1: Musical Composition

Working in pairs, please work through the [Hello Magenta.ipynb](https://colab.research.google.com/notebooks/magenta/hello_magenta/hello_magenta.ipynb) notebook that can be found on Google Colab:

https://colab.research.google.com/notebooks/magenta/hello_magenta/hello_magenta.ipynb

Attempt the following things:

1. Create your own note sequence(s)
2. Adjust the length of the input sequence, num_steps, and temperature
3. Does a longer or shorter input sequence lead to better results?
4. Does a longer or shorter num_steps lead to better results?
5. How does adjusting the temperature influence the result?
6. Interpolate between two and more sequences, adjusting the length
7. What parameters allow you to adjust interpolation?
8. How is interpolation related to composition?

### Local Install

To install the dependencies for Magenta to run the notebook locally, you need several OS-specific packages.

For Mac OS X:

    $ brew install fluidsynth

For Ubuntu Linux:

    $ sudo apt-get install build-essential libasound2-dev libjack-dev portaudio19-dev

For Windows: Unfortunately, to install fluidsynth on Windows, you have to build the package yourself, there doesn't seem to be any prebuilt binaries. See the [build instructions for FluidSynth on Windows](https://github.com/FluidSynth/fluidsynth/wiki/BuildingWithCMake#building-with-msys2-on-windows) to compile it locally. Note that these notebooks are untested on Windows, so I'm not sure what other dependencies are required.

Once you've installed FluidSynth:

    $ pip install magenta jupyter python-rtmidi

Or alternatively you can install all the dependencies using `pip install -r requirements.txt`. This may take some time, but after install you should be able to run the `music.ipynb` notebook.


## Workshop 2: Deep Dream and Lucid

- [DeepDream TensorFlow](https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/tutorials/generative/deepdream.ipynb)
- [TensorFlow Lucid](https://colab.research.google.com/github/tensorflow/lucid/blob/master/notebooks/tutorial.ipynb)