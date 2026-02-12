# dl-homework1-mnist-kfold

# Homework 1 – MNIST Hyperparameter Tuning with 4‑Fold Cross Validation

This repository contains my solution for Homework 1 of CSE 547 (Deep Learning).  
The assignment focuses on optimizing neural network hyperparameters using **4‑fold cross validation** on the MNIST dataset.

---

## Objectives
- Train multiple neural network architectures on MNIST
- Perform **4‑fold cross validation** using only the training set
- Compare:
  - 1‑layer network (1 node)
  - 2‑layer network (12 nodes, 4 nodes)
  - 3‑layer network (32, 32, 16 nodes)
- Evaluate 3 learning rates: **0.1**, **0.001**, **0.00001**
- Select the top 3 models based on validation accuracy
- Evaluate the top models on the test set and compare rankings

---

## Repository Contents
- **`CSE 547-Homework 1-checkpoint.ipynb`** — Full Jupyter Notebook with all code (runs independently)
- **`CSE 547 HW 1.ppt`** — Final report summarizing experiments, plots, and results
- **`https://louisville.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=96c7ed91-9d49-4e38-bbfc-b3e80178693d&start=0.551312`** — Link to the Panopto presentation video

---

## Methods & Experiments

### **1. Hyperparameter Search**
Tested combinations of:
- **Architectures:**  
  - 1 layer (1 node)  
  - 2 layers (12, 4)  
  - 3 layers (32, 32, 16)
- **Learning rates:**  
  - 0.1  
  - 0.001  
  - 0.00001

### **2. Cross Validation**
- Performed **4‑fold CV** on the training set  
- For each fold and each configuration:
  - Tracked training accuracy  
  - Tracked validation accuracy  
  - Plotted accuracy curves  

### **3. Model Selection**
- Computed **average validation accuracy** across folds  
- Selected the **top 3** hyperparameter configurations

### **4. Final Evaluation**
- Trained each top model on the full training set  
- Generated predictions on the test set  
- Compared:
  - Test accuracy  
  - Validation ranking  
  - Consistency between validation and test performance

---

## Video Presentation
A 10‑minute walkthrough of:
- The Jupyter Notebook (first 5 minutes)
- The report and results (last 5 minutes)

Panopto link:  
https://louisville.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=96c7ed91-9d49-4e38-bbfc-b3e80178693d&start=0.551312
