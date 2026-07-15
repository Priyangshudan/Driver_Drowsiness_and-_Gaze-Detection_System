# Driver_Drowsiness_and-_Gaze-Detection_System
STEPS TO RUN OUR PROJECT
        STEP 1) Install Python 3.11.9 to run the project.
STEP 2) Load all files in VSCODE in this arrangement:
 
STEP 3) Install shape_predictor_68_face_landmarks.dat 
http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2
and add it in the “models” folder as shown.
STEP 4) Install ffmpeg-8.0-essentials_build 

1: Install the ZIP Folder
On Windows:
1.	Go to: https://www.gyan.dev/ffmpeg/builds/
2.	Scroll down to the "release builds" section.
3.	Download the file named ffmpeg-release-essentials.zip.
2: Unzip and Place the Folder
First, we'll extract the program and move it to a permanent, simple-to-find location.
1.	Extract: Right-click the ffmpeg-release-essentials.zip file and choose "Extract All...".
2.	Rename & Move: This will create a new folder with a long name (like ffmpeg-7.0-essentials_build). For simplicity, please rename this folder to just ffmpeg.
3.	Move this ffmpeg folder to a permanent location. The easiest place is the root of your C:\ drive. The final path for the folder should be C:\ffmpeg.
3: Add the Program to your System PATH
This is the most important step. We need to add the program's location to the Windows "Path" so the command prompt (and our Python script) can find it.
1.	Copy the Path: The folder inside C:\ffmpeg that we need is named bin. The full path you need to copy is: C:\ffmpeg\bin
2.	Open Environment Variables: In your Start Menu, type environment variables and select "Edit the system environment variables" from the results.
3.	Navigate: In the "System Properties" window that opens, click the "Environment Variables..." button at the bottom.
4.	Edit Path: In the new window, look at the top box ("User variables for..."). Find and select the variable named "Path", then click the "Edit..." button.
5.	Add New Path: Click the "New" button. This will create a new blank line. Paste the path you copied in Step 2.1: C:\ffmpeg\bin
6.	Save: Click "OK" on all three windows to close and save the changes.
4: Verify the Installation
To confirm it worked, you must restart your terminal or code editor.
1.	Restart: Please close and re-open your terminal (e.g., Command Prompt, PowerShell, or VS Code). This is critical for it to load the new settings.
2.	Verify: In the new terminal, type the following command and press Enter: ffmpeg -version
If the installation was successful, you will see text displayed about the FFmpeg version and its configuration. If it says "command not found," something went wrong in Step 2.
	STEP 5) Create the “pages” folder as shown above and in it place the files “summary.py” and “dashboard.py” 
	STEP 6) Install all the required modules by “pip install -r projectrequirements.txt”
	STEP 7) Run “python calibrate.py” in the VS Code terminal to get your own model saved in the folder “models” and calibrate the system according to the user’s face dimensions.
	STEP 8) Run “python detect.py” in the VS Code terminal to run the total detection program. The “clips” and “recording” folder are created automatically by the system once the detection program ends. The “recording” folder contains the CSV files along with the .avi recordings of the detection program run on the user.
	STEP 9) Run “streamlit run app.py” to get the streamlit dashboard on your browser.

