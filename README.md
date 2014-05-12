audiosearchengine
=================

Requirements

	*Python Ver. 3.X.X
	*python-tk package for GUI application
	*X11 (for Cygwin) or XQuartz installed (for Mac) when using GUI application
	*WAV audio file (.wav) format: signed mono 16 bit PCM
		Use .wav converters online, and if neccessary re-sample the audio files
		using Audacity Opensource Software 
		For UNIX users, you may also use SoX to add .wav header to raw bit stream data

Screenshots?
	
	screenshot.png is available in img directory

What is it?

	Suppose you have a recorded section of some audio file, but
	you cannot remember the song name or the ring-tone name. You can search
	for similar audio files in the database with the best waveform alignments. 
	
	You can adjust the level of stringency to balance the speed and quality of
	the search.
	
	The algorithm implements a Map-Reduce pattern with multiple map processes
	that run in parallel.

Python Libraries Used

	tkinter (for GUI)
	multiprocessing

How to use

	You can run either interfaceCMD.py and interfaceGUI.py. interfaceCMD.py is for
	command line use and interfaceGUI.py is for GUI. On the GUI application,
	you can also compare the two waveforms.

	Place query wav file in the top level directory where interfaceCMD.py is stored.
	Run search by running interfaceCMD.py. You can also add .wav files to the
	db directory (database). 

	Please note that the algorithm is designed for Python Version 3.X.X. (interfaceCMD.py).
	If possible, run interfaceCMD.py with python3.

