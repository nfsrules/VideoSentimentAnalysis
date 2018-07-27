# VideoSentimentAnalysis
Implementation of gender and sentiment recognition on real-time video streams. 

## Installation

1. <strong>Install dlib v19.9</strong>

Pre-requisites:
* Have Python 3 installed. On macOS, this could be installed from homebrew or even via standard Python 3.6 downloaded installer from https://www.python.org/download. On Linux, just use your package manager.

* On macOS:
    * Install XCode from the Mac App Store (or install the XCode command line utils).
    * Have homebrew installed
* On Linux:
    * For a full list of apt packages required, check out the example Dockerfile and copy what's installed there.
    * These instructions assume you are using Ubuntu 16.04 or newer. If you are using 14.04, you can try these installation instructions instead to work around the old CMake version.
* These instructions assume you don't have an nVidia GPU and DON’T have Cuda and cuDNN installed and don't want GPU acceleration (since none of the current Mac models support this).


Clone repository:

`git clone https://github.com/davisking/dlib.git`


Build dlib for Python 3:

`cd dlib
mkdir build; cd build; cmake .. -DDLIB_USE_CUDA=0 -DUSE_AVX_INSTRUCTIONS=1; cmake --build .`

`cd ..
python3 setup.py install --yes USE_AVX_INSTRUCTIONS --no DLIB_USE_CUDA`

Verify by running `python3` and type `import lib`

2. <strong>Clone repository and install Face Recognition toolbox</strong>

Clone Axionable repository
`git clone https://github.com/Axionable/RealTimeEmotion`

Install face_recognition
`pip3 install face_recognition`


3. <strong>Run Real-time Emotion Recognition notebook</strong>


## Credits
	Dlib XXXX
	Facial recognition python

