xacro2urdf
=====

[Parser]() for xacro to urdf based on [saulrh/xacro](https://github.com/saulrh/xacro). This `xacro.py` can be executed without ROS environment.

## My Environment
+ windows 8.1 
+ python3.6 with Anaconda
+ Visual Studio Code

## How to use
Run `test_xacro.py` to verify that the `xacro.py` is working properly.

**Attention:** the `xacro.py` must be in same directory as `urdf` file

## What's difference from [saulrh/xacro](https://github.com/saulrh/xacro) code

Because [saulrh/xacro](https://github.com/saulrh/xacro) code need python2 environment and works incorrectly in my computer, so I convert the code from python2 to python3 and fix some bugs in file path reading.
