xacro2urdf
=====

Parser([xacro.py](https://github.com/doctorsrn/xacro2urdf/blob/master/xacro.py)) for xacro to urdf based on [saulrh/xacro](https://github.com/saulrh/xacro). This `xacro.py` can be executed without ROS environment.

## My Environment
+ windows 8.1 
+ python3.6 with Anaconda
+ Visual Studio Code

## How to use
1. Run `test_xacro.py` to verify that the `xacro.py` is working properly.
2. Run `python xacro.py` can get some helpful information.
3. Move `xacro.py` to the same directory as `urdf` folder. You can see the file structure in [abb_irb4600_support](https://github.com/doctorsrn/xacro2urdf/tree/master/abb_irb4600_support) folder for detail.
4. Run `python xacro.py -o ./target.urdf urdf/origin.xacro` to start convertion. For example, `python xacro.py -o ./test_abb_4600.urdf urdf/irb4600_60_205.xacro` in [abb_irb4600_support](https://github.com/doctorsrn/xacro2urdf/tree/master/abb_irb4600_support) folder. If convert successfully, the `test_abb_4600.urdf` will be generated.

**Attention:** The `xacro.py` must be in same directory as `urdf` folder.

## What's difference from [saulrh/xacro](https://github.com/saulrh/xacro) code

Because [saulrh/xacro](https://github.com/saulrh/xacro) code need python2 environment and works incorrectly in my computer, so I convert the code from python2 to python3 and fix some bugs in file path reading in line 378. You can see the change through the comments.