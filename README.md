# avatrify
Real-Time Deepfake Avatars for Windows
Avatars for video calls - set up for Windows.

Based on:

Avatarify adapted for Windows.
First Order Motion Model for generating avatars.
Requirements

conda
CUDA
Performance:

Windows (with 1080 Ti GPU): ~30 fps
Guide

▶️ YOUTUBE TUTORIAL

Install

Download

Download model's weights from Google Drive [716 MB] or from Mega [716 MB]
Place vox-adv-cpk.pth.tar file in the root directory
Windows

Setup avatarify conda environment with all required dependencies. Open your miniconda command prompt, navigate to the avatarify-windows folder and run: install.bat
Now execute run.bat - you should now see the application running, and two windows will appear, if everything is working correctly.
To output to webcam, download and install OBS
Download and install the latest Windows release of OBS-VirtualCam
Reboot.
You are now able to use OBS to capture the output window of Avatarify, and output your result to a virtual webcam.
Setup avatars

Copy your avatars into avatars folder. Crop pictures to make them square. Prefer pictures with uniform background.

Run

Your web cam must be plugged-in. You can choose your camera when running run.bat

Controls

Keys	Controls
1-9	These will immediately switch between the first 9 avatars.
0	Toggles avatar display on and off.
A/D	Previous/next avatar in folder.
W/S	Zoom camera in/out.
Z/C	Adjust avatar target overlay opacity.
X	Reset reference frame.
F	Toggle reference frame search mode.
R	Mirror reference window.
T	Mirror output window.
Tips

It is recommended to use the avatar overlay and the zoom in/out function to align your face in the preview window as closely as possible in proportion and position to the target avatar. When you have aligned, hit 'X' to use this frame as reference to drive the rest of the animation.

Alternatively, you can hit 'F' for the software to attempt to find a better reference frame itself. This will slow down the framerate, but while this is happening, you can keep moving your head around: the preview window will flash green when it finds your facial pose is a closer match to the avatar than the one it is currently using. You will see two numbers displayed as well: the first number is how closely you are currently aligned to the avatar, and the second number is how closely the reference frame is aligned.

You want to get the first number as small as possible - around 10 is usually a good alignment. When you are done, press 'F' again to exit reference frame search mode.

You don't need to be exact, and some other configurations can yield better results still, but it's usually a good starting point.

Skype

Go to Settings -> Audio & Video, choose OBS-Camera camera.

Zoom

Go to Settings -> Video and choose OBS-Camera from Camera drop-down menu.

Slack

Make a call, allow browser using cameras, click on Settings icon, choose OBS-Camera in Video settings drop-down menu.

Discord

Go to User Settings -> Voice & Video, choose OBS-Camera from Camera drop-down menu.
