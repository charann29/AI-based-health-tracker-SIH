# AI Based Health Tracker
Our idea attempts to keep track and monitor the process of mid-day meals for students whether they are receiving the necessary calories and nutrients intake along with attendance.
<br><br>
**Tech Stack** <br><br>
![Flask](https://img.shields.io/badge/-Flask-blue?style=for-the-badge&logo=Flask)
![Python](https://img.shields.io/badge/-Python-black?style=for-the-badge&logo=Python)
![MongoDB](https://img.shields.io/badge/-MongoDB-black?style=for-the-badge&logo=mongodb)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
<br><br>
**Video of the project** <br><br>
[![Watch the video](https://user-images.githubusercontent.com/55660103/180276164-9ce5d3f7-5e65-42de-a255-b80349b4113b.png)](https://www.youtube.com/watch?v=1CnxmrVq94Y)
<br><br>
<h3>Idea/Approach Details</h3>
<ul>
<li>In an attempt to answer PM’s call for Anaemia Mukt Bharat.
<li>Track and monitor the weekly menu, calories and protein intake per child everyday using our model.
<li>Verify that children are attending the school and receiving a minimum nutrient meal for their physical and cognitive growth.
<li>Provide a dashboard to help gain insights by Monitoring and keeping track of the health of students as well as provide a streaming 
<li>service if requested for the interested authorities to check the status of the program .
</ul>

### Face Recognition for Attendance Tracking

_You can also read a translated version of this file [in Chinese 简体中文版](https://github.com/ageitgey/face_recognition/blob/master/README_Simplified_Chinese.md) or [in Korean 한국어](https://github.com/ageitgey/face_recognition/blob/master/README_Korean.md) or [in Japanese 日本語](https://github.com/m-i-k-i/face_recognition/blob/master/README_Japanese.md)._

Recognize and manipulate faces from Python or from the command line with
the world's simplest face recognition library.

Built using [dlib](http://dlib.net/)'s state-of-the-art face recognition
built with deep learning. The model has an accuracy of 99.38% on the
[Labeled Faces in the Wild](http://vis-www.cs.umass.edu/lfw/) benchmark.

This also provides a simple `face_recognition` command line tool that lets
you do face recognition on a folder of images from the command line!


[![PyPI](https://img.shields.io/pypi/v/face_recognition.svg)](https://pypi.python.org/pypi/face_recognition)
[![Build Status](https://github.com/ageitgey/face_recognition/workflows/CI/badge.svg?branch=master&event=push)](https://github.com/ageitgey/face_recognition/actions?query=workflow%3ACI)
[![Documentation Status](https://readthedocs.org/projects/face-recognition/badge/?version=latest)](http://face-recognition.readthedocs.io/en/latest/?badge=latest)

## Features

#### Find faces in pictures

Find all the faces that appear in a picture:

![](https://cloud.githubusercontent.com/assets/896692/23625227/42c65360-025d-11e7-94ea-b12f28cb34b4.png)

```python
import face_recognition
image = face_recognition.load_image_file("your_file.jpg")
face_locations = face_recognition.face_locations(image)
```

#### Find and manipulate facial features in pictures

Get the locations and outlines of each person's eyes, nose, mouth and chin.

![](https://cloud.githubusercontent.com/assets/896692/23625282/7f2d79dc-025d-11e7-8728-d8924596f8fa.png)

```python
import face_recognition
image = face_recognition.load_image_file("your_file.jpg")
face_landmarks_list = face_recognition.face_landmarks(image)
```

Finding facial features is super useful for lots of important stuff. But you can also use it for really stupid stuff
like applying [digital make-up](https://github.com/ageitgey/face_recognition/blob/master/examples/digital_makeup.py) (think 'Meitu'):

![](https://cloud.githubusercontent.com/assets/896692/23625283/80638760-025d-11e7-80a2-1d2779f7ccab.png)

#### Identify faces in pictures

Recognize who appears in each photo.

![](https://cloud.githubusercontent.com/assets/896692/23625229/45e049b6-025d-11e7-89cc-8a71cf89e713.png)

```python
import face_recognition
known_image = face_recognition.load_image_file("biden.jpg")
unknown_image = face_recognition.load_image_file("unknown.jpg")

biden_encoding = face_recognition.face_encodings(known_image)[0]
unknown_encoding = face_recognition.face_encodings(unknown_image)[0]

results = face_recognition.compare_faces([biden_encoding], unknown_encoding)
```

You can even use this library with other Python libraries to do real-time face recognition:

![](https://cloud.githubusercontent.com/assets/896692/24430398/36f0e3f0-13cb-11e7-8258-4d0c9ce1e419.gif)

See [this example](https://github.com/ageitgey/face_recognition/blob/master/examples/facerec_from_webcam_faster.py) for the code.
