# Recording-with-Multiple-Cameras
This project employs PyQt5 to design a UI with functionalities for adding, editing, and deleting cameras, as well as recording. It simultaneously opens multiple cameras using threads and FrameBuffer. Additionally, it utilizes the Schedule library to record new videos every day at midnight. Finally, the program is packaged into an executable file. This application can be utilized for data collection before deep learning annotation.

<div align="center">
    <img src="https://github.com/KennyChen880127/YOLOv8-PY-to-EXE/blob/master/result.jpg" alt="mainScreen"><br>
    Main Screen
</div>


## Instructions

* Note: After the program executes, it will create "SaveLog" and "Video Record" folders in the same directory. The "SaveLog" folder is for storing log records, while the "Video Record" folder is for storing recorded videos. Additionally, it will create a "data.ini" file containing all camera data.

* Camera Addition: Pressing the "Add Camera" button will prompt a window where you can input the camera source (it can be a number or an RTSP link), then input the camera name, and finally, press "Save".

<div align="center">
    <img src="https://github.com/KennyChen880127/YOLOv8-PY-to-EXE/blob/master/result.jpg" alt="mainScreen"><br>
    Camera Addition Screen
</div>

* Camera On/Off: Pressing the "On/Off" button will toggle the camera's status. If the camera doesn't start after a while, please ensure that the source is correct. If there's an error, you can press the "Edit" button to make changes or press the "Delete" button to remove this data.

* Start/Stop Recording: Pressing "Start Recording" will initiate video recording for the selected camera in the ComboBox. New recordings will also be scheduled to start at midnight (00:00). Pressing "Stop Recording" will stop video recording, but the camera will continue to display the live feed.

* Edit Camera: Pressing the "Edit" button will allow you to edit the currently selected camera data in your ComboBox. You can enter a new source or camera name.

* Delete Camera: Pressing the "Delete" button will remove the currently selected camera data from your ComboBox.

