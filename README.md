# 📷 3D Vision — Camera Projection, Pose Estimation & 3D Reconstruction  
SIT789 — Robotics, Computer Vision and Speech Processing  
**Pass Task 6.1**

This project implements fundamental components of **3D computer vision**, including:

- Pin-hole camera modelling  
- 3D→2D projection  
- Camera pose estimation using SVD  
- 3D reconstruction using Structure-from-Motion (SfM)  
- SIFT keypoint extraction, feature matching, RANSAC, triangulation  
- Visualisation of reconstructed 3D point clouds

The implementation follows the requirements of **SIT789 Task 6.1**.

---

## 📌 Objectives

The goal of this project is to practise and understand:

### ✔ 1. **3D Projection**  
Using the pin-hole camera model  
\[
P = K [R | t]
\]  
Projecting 3D world points into 2D image coordinates.

### ✔ 2. **Camera Pose Estimation**  
Recovering the camera matrix **P̂** from corresponding 3D and 2D points using:

- Construction of the linear system **A p = 0**
- Singular Value Decomposition (SVD)
- Selection of p as the eigenvector corresponding to the smallest singular value
- Quantitative evaluation by projection distance error

### ✔ 3. **3D Reconstruction (Structure-from-Motion)**  
Using two calibrated views:

- Extract SIFT features  
- Match descriptors with BFMatcher  
- Estimate Essential Matrix using RANSAC  
- Recover second camera matrix **P₂**  
- Triangulate matched points  
- Visualise the reconstructed 3D structure

---

## 📂 Project Structure

