# Google Assistant with Face Recognition Trigger Support


## Description:

We forked the open-source assistant-sdk-python project and extended it to enable users to trigger face recognition of the DIY Mirror using voice command.


## Implementation:

* "pushtotalk.py" is modified to support face recognition trigger
* "pi_face_recognition.py" performs OpenCV face recognition and returns the recognized user
* "my_recog_run.sh" runs "pi_face_recognition.py"
* "my_import.sh" activates the virtual environment and prepares for OpenCV operations


## Execution:

```sh
cd google-assistant-sdk/googlesamples/assistant/grpc
. my_import.sh
python pushtotalk.py
```


## Usage:

Before interaction with Google Assistant, press "enter" key in the command line window. Then speak "Talk to DIY Mirror" and "Face Recognition" in turn to trigger the Python script for face recognition.


## References:
Concerning the usage of OpenCV-based face recognition library in "pi_face_recognition.py", we referred to the tutorial on the following website:

- Raspberry Pi Face Recognition: https://www.pyimagesearch.com/2018/06/25/raspberry-pi-face-recognition/