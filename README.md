# Nano Fuse CAD Modelling using Build123d

## Overview

This project demonstrates the complete CAD modelling workflow of a **Nano Fuse** using the Python-based parametric CAD library `build123d`.

Instead of designing the geometry manually in traditional CAD software, the entire structure is created programmatically using Python. Every dimension, extrusion, cut, chamfer, and fillet is controlled through parameters, making the design fully reproducible, customizable, and scalable.

The goal of this project was to explore how computational design can be used to build complex nano-scale structures with clean and modular code.

---

## What This Project Does

The script builds the nano fuse step-by-step by combining multiple geometric components:

* A tapered base structure
* Top support blocks
* Precision cut sections
* Mid connector structures
* Bottom attachment plates
* Side protrusions and side extrusions
* Fillets and chamfers for realistic finishing

Each section is created independently and then combined into a final manufacturable 3D model.

---

## Workflow of the Code

### 1. Parametric Design Setup

The project starts by defining all geometric dimensions as parameters.

This makes the model:

* Easy to modify
* Fully scalable
* Reusable for future design iterations

---

### 2. Plane Construction

Custom reference planes are created to accurately position different nano fuse components.

These planes act as construction guides for:

* Left and right top structures
* Mid sections
* Side attachments
* Precision cut regions

---

### 3. Base Geometry Creation

The bottom structure is generated first using polygon sketches and extrusion operations.

This creates the primary foundation of the nano fuse.

---

### 4. Feature Modelling

Additional structures are progressively added:

* Top blocks
* Mid attachments
* Connector regions
* Side components

Boolean subtraction is used to create internal cuts and fine structural details.

---

### 5. Surface Refinement

Fillets and chamfers are applied to improve:

* Structural smoothness
* Edge transitions
* Realistic CAD finishing

This gives the final model a cleaner engineering appearance.

---

### 6. Final Export

The completed model is exported as an `.stl` file for:

* 3D visualization
* Simulation workflows
* Additive manufacturing pipelines

---

## Technologies Used

* Python
* build123d
* Parametric CAD Modelling


---

## Output

The generated CAD models and exported files can be found in the repository output section:

* `Final_Part.stl` → Final 3D printable nano fuse model
* Source Python script → Complete parametric CAD workflow implementation

You can directly access the files here:

* [STL Output File](./Final_Part.stl)
* [Source Code](./Build_Code.py)

These files demonstrate the complete programmatic modelling pipeline built using `build123d`.


```python
export_stl(Final_Part.part, "Final_Part.stl")
```

---

