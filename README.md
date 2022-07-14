# refactored-adventure
## Training Detectron2  with Custom COCO Datasets.

In this repository, I have implemented how Detectron2 can be used in the field of computer vision and object detection. Detectron2 is a platform for object detection, segmentation and other visual recognition tasks.

### What is Detecron 2?
Detectron2 is Facebook AI Research's next generation library that provides state-of-the-art detection and segmentation algorithms. It is the successor of Detectron and maskrcnn-benchmark. It supports a number of computer vision research projects and production applications in Facebook.

Before moving on with the implementation, please setup workspace by installing required dependancies. So, open up jupyter notebook, start a python kernel and proceed with below instructions.
First install detectron2's dependancies:
```python
!pip install cython pyyaml==5.1
!pip install -U 'git+https://github.com/cocodataset/cocoapi.git#subdirectory=PythonAPI'
```
Then install Detectron2, detectron2-ResNeSt, centermask2, etc:
```python
%cd /content/
!git clone https://github.com/facebookresearch/detectron2
%cd /content/detectron2
!pip install -r requirements.txt
!python setup.py install
!pip install git+https://github.com/facebookresearch/fvcore.git
```
```python
%cd /content/
!python -m pip install 'git+https://github.com/zhanghang1989/detectron2-ResNeSt.git'

%cd /content/
!git clone https://github.com/zhanghang1989/detectron2-ResNeSt
```
```python
%cd /content/
!pip install detectron2==0.3 -f https://dl.fbaipublicfiles.com/detectron2/wheels/cu101/torch1.5/index.html
!git clone https://github.com/youngwanLEE/centermask2
```
