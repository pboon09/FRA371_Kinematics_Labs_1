# FRA371_Kinematics_Labs_1

![Course](https://img.shields.io/badge/Course-FRA371-blue)
![Lab](https://img.shields.io/badge/Lab-1-green)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)

Complete [Lab 1 Part B](Lab1_PartB.ipynb) before the time ends!

## Instructions

Open `Lab1_PartB.ipynb` and select the Python kernel that matches the version where the required libraries are installed.

### Part 1: Check Hand Calculation with the Library

- Enter the assigned point **M** in the section marked with `# edit here`.
- Enter the joint values for each joint (radians/meters) in the sections marked with `# edit here`.

**Expected result:**
- The tip position should be close to point **M**.
- The error should be close to **0**.

### Part 2: Build Your Model and Compute Forward Kinematics (FK)

- Fill in the **modified Denavit–Hartenberg (mDH)** parameter table.

**Expected result:**
- The completed mDH table should match the values obtained in **Part A3**.

- Modify `q_A` according to the robot's joint types.
- In the section marked with `# edit here to compute T, tip, and dist for q_A and q_B`, write code to compute:
  - the transformation matrix (`T`),
  - the end-effector position (`tip`), and
  - the distance (`dist`) from the end effector to point **M**,

  as completed in **Part A5**.

**Expected result:**
- The program output should match your hand calculations.

### Part 3: Cross-check Your mDH Model vs. Your URDF Model

- Run the notebook and compare the robot generated from the **URDF** model with the one generated from the **mDH** parameters.

**Expected result:**
- The end-effector positions from both models should be nearly identical.

## Submit your answer
Copy cell output of each part and paste them in [answer sheet file](ANSWER.md)

## Conditions

- Use **only** the functions and syntax specified in the lab instructions.
- Add or modify code **only** in lines marked with `# edit here` or `# YOUR TURN`.
- Turn off **Wi-Fi** during the lab.