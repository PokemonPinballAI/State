NAMES:
George Lim
Jarod Nakamoto
Kenneth-Matthew Velarde
Daniel Gruhn

REPORT NAME:
Pokemon Pinball Final Report
-----------------------------------------------------------------------------------------
CODE:
Dependencies:
	-Python 3.6 (Keras is not compatible with 3.7)
	-gym-retro	 https://github.com/openai/retro
	-h5py 	http://docs.h5py.org/en/latest/quick.html
	-keras + a backend 	https://keras.io
	-keras-rl	https://github.com/keras-rl/keras-rl
	-easydict 	https://pypi.org/project/easydict/1.2
	-skimage 	http://dx.doi.org/10.7717/peerj.453
	-ffmpeg(for video) after installation you will need to set a path in the command line to the bin file of ffmpeg see https://github.com/adaptlearning/adapt_authoring/wiki/Installing-FFmpeg

–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––-
There are 2 files included:
 -Testing_pokemonpinball.ipynb is our main script using keras neural networks to decide what actions to take in our gym retro environment. 
  One of the requirements of keras is the implementation of a learning library (we used tensorflow). 
  Our program is based off of the keras-rl library, which also requires h5py as a supplementary library. 
  Since we used jupyter notebook to run our python code, we had to use the EasyDict library to store what would have been arguments of a normal python script that were not compatible with Juptyer. 
  We chose Jupyter notebook to run our code because of its functionality of running select blocks of code was more efficient than having to recompile, rebuild the game environment, and run everything. 
  We used skimage to render our game frames into gray-scale. The Testing_pokemonpinball file generates .bk2 files in it’s file location after completing a learning epoch which are later used to create replays of trials.


 -With the assistance of our good friend, Kendall of Team Mario, we were able to create a way to convert the .bk2 files make by our test program to viewable movies with our Movie_Converter.ipynb script. 
  The movie converter script utilizes gym retro’s built in playback and render to video functions, which required ffmpeg to run. 
  After running the testing program, you can choose to convert a specific replay into an mp4 for visual review. 



-----------------------------------------------------------------------------------------------------------------
DATA:
Link to some weights generated - https://drive.google.com/file/d/1LgDtSlM0nt6ADDE7CDopj7FMW43b4gxv/view?usp=sharing

Given the fact that we had issues with implementing the learning algorithm, we currently do not have much data on hand to present. 
We do have two video files however showing a training epoch and the stalling in our tests. 



