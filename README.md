# ProForm
Frontend implementation of video pose similarity to analyze similarities between two motions<br>

# How to Use
You need dependencies below.

- python3
- tensorflow 1.4.1+
- opencv3, protobuf, python3-tk
- slidingwindow
  - https://github.com/adamrehn/slidingwindow

Install 3rd party requirements
```bash
$ git clone https://www.github.com/ildoonet/tf-pose-estimation
$ cd ProForm
$ pip3 install -r requirements.txt
```

Build c++ library for post processing. See : https://github.com/ildoonet/tf-pose-estimation/tree/master/tf_pose/pafprocess
```
$ cd tf_pose/pafprocess
$ swig -python -c++ pafprocess.i && python3 setup.py build_ext --inplace
```

Replace project in Apache Folder
