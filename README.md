# FRA371_Kinematics_Labs_1

![Course](https://img.shields.io/badge/Course-FRA371-blue)
![Lab](https://img.shields.io/badge/Lab-1-green)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)

## Robot Setup

Add your own robot to this project and confirm it loads.

### 1. Move your robot into `my_robot/`

Your robot comes from a **URDF exporter** (your CAD tool): one `.urdf` file and a set
of `.stl` meshes.

1. Put your mesh files in `my_robot/meshes/`.
2. Save your URDF as `my_robot/robot.urdf`.

### 2. Re-path the meshes

In `my_robot/robot.urdf`, every mesh path **must** look like this:

```xml
<mesh filename="package://my_robot/meshes/YOUR_FILE.stl"/>
```

## Instructions

Open [Lab 1 Part B](Lab1_PartB.ipynb) and select the Python kernel that matches the version where the required libraries are installed.

### Part 1: Build Your Model

- Fill in the **modified Denavit–Hartenberg (mDH)** parameter table.

**Expected result:**
- The completed mDH table should match the values obtained in **Part A3**.

### Part 2: Compute Forward Kinematics (FK)

- Modify `q_A` and `q_B` according to the robot's joint types.
- In the section marked with `# edit here to compute T and tip for q_A and q_B`, write code to compute:
  - the transformation matrix (`T`),
  - the end-effector position
  - the end-effector orientation

**Expected result:**
- The program output should match your hand calculations.

### Part 3: Cross-check Your mDH Model vs. Your URDF Model

- Run the notebook and compare the robot generated from the **URDF** model with the one generated from the **mDH** parameters.

**Expected result:**
- The end-effector positions and orientations from both models should be nearly identical.

## Submit your answer
Copy cell output of each part, rename the file to your group number, and paste them in [answer sheet file](ANSWER_GNN.md)

## Conditions

- There will be **reference of the functions and syntax** that can help you write down in the file.
- Add or modify code **only** in lines marked with `# edit here`
- Turn off **Wi-Fi** during the lab.