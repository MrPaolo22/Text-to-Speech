Team number: xohw23-170

Project name: Text to speech

Link to YouTube Video(s):

Link to project repository:

 

University name: Sapienza

Participant(s): Paolo Russo

Email: russo.1919141@studenti.uniroma1.it

Supervisor name: Antonio Mastrandrea

Supervisor e-mail: PSDsapienza@gmail.com

 

Board used: ZYBO Z7 ZYNQ-7020

Software Version: 1.0

Brief description of project: The goal was creating a simple Italian text to speech with light datasheet. This data can be generated for any type like 8 bits, 16 bits or float with MATLAB. Because of the Zybo board audio decoder settings it can receive only 24 bits fixed point data so we created data compatible with that.

 

Description of archive (explain directory structure, documents and source files): Here are proposed only the path with files that have been modified
|--vitis/
|  |--.analytics
|  |--IDE.txt
|  |--text2speech_system/
|  |--.metadata/
|  |--text2speech/				   
|  |  |--src/		     
|  |  |  |--demo.c
|  |  |  |--demo.h
|  |  |  |--soundsdata.h
|  |  |  |--audio/
|  |  |  |  |--audio.c
|  |  |	 |  |--audio.h	
|  |--RemoteSystemsTempFiles/
|  |--system_wrapper.xsa
|--generate_rec_data.mlx
|--funcs.mlx
|--Italian phonemes.mat
|--readme.txt
|--Project_Report.pdf

Instructions to build and test project

Step 1:
Open generate_rec_data on MATLAB and Play the script by loading "Italian phonemes.mat".
Step 2:
Open funcs on MATLAB and Play this script, it will generate the test sentence "Ciao sono Paolo" as gen_data.
Step 3:
Open with Vitis the project named "vitis" and build it.
Step 4:
Once the board is linked to the PC Play the project inside.
Step 5:
Press BTN2 in order to play the desired sound.