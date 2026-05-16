# Fetch Task and Motion Planning using Control Barrier Functions

**Summary:** A Task and Motion Planning (TAMP) framework using Control Barrier Functions (CBF) to guide a Fetch robot through a mission while actively avoiding dynamic obstacles meant to be human beings in real-time.

**Files:**

* `fetch_tamp.ipynb`: Core simulation, kinematics, TAMP state machine, and CBF safety filter.
* `cbf_multi_eval.png`: Output plot evaluating robot-to-obstacle safety distances.

**How to Reproduce:**

1. **Install dependencies:**
```bash
conda install pinocchio -c conda-forge
pip install meshcat meshcat-shapes robot_descriptions ipywidgets scipy matplotlib

```

2. **Execute the simulation:** Run the cells in the Jupyter Notebook.
3. **Visualize in 3D:** Open the Meshcat URL printed in your terminal (typically `http://127.0.0.1:7000/static/`) to watch the robot navigate.
4. **View Results:** Upon completion (30 seconds / 600 steps), the script will automatically generate and save `cbf_multi_eval.png` to your directory.
