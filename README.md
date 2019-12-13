# Hello SMPL

[SMPL](https://smpl.is.tue.mpg.de/) is A Skinned Multi-Person Linear Model.

![image](https://github.com/foamliu/Hello-SMPL/raw/master/images/smpl.png)

## Dependencies
- Python 3.6.8
- PyTorch 1.3.0

## Models
Download following two SMPL models -> models folder:
- basicModel_f_lbs_10_207_0_v1.0.0.pkl
- basicmodel_m_lbs_10_207_0_v1.0.0.pkl

## Usage

1.Hello World code

This script demonstrates a few basic functions to help users get started with using 
the SMPL model. The code shows how to:
  - Load the SMPL model
  - Edit pose & shape parameters of the model to create a new body in a new pose
  - Save the resulting body as a mesh in .OBJ format

```bash
$ python hello_smpl.py
..Output mesh saved to:  ./hello_smpl.obj
```

You can visualize it like this:

![image](https://github.com/foamliu/Hello-SMPL/raw/master/images/hello_smpl_ouput.jpg)


2.Render code

This script demonstrates loading the smpl model and rendering it using OpenDR 
to render and OpenCV to display (or alternatively matplotlib can also be used
for display, as shown in commented code below). 

This code shows how to:
  - Load the SMPL model
  - Edit pose & shape parameters of the model to create a new body in a new pose
  - Create an OpenDR scene (with a basic renderer, camera & light)
  - Render the scene using OpenCV / matplotlib
  
 ```bash
$ python render_smpl.py
..Output mesh saved to:  ./hello_smpl.obj
```