# Julia_codes
learning and trial for Julia.

## Table of Contents

* [About the Project](#About)
* [Dataset analysis](#dataset)
* [Results](#results)
* [Acknowledgement](#Acknowledgement)

## About the Project
This is a Julia code of applying RANSAC on [Toronto-3D DATASET](https://github.com/WeikaiTan/Toronto-3D?tab=readme-ov-file#download). 
  
## Dataset analysis
  * View of the RGB and intensity heatmap data
    <img width="1487" alt="Screenshot 2024-11-13 at 9 51 23 pm" src="https://github.com/user-attachments/assets/19b2b814-b17f-48d3-9512-d9cfc0ce9cd4">
  * Take one point in L0004.ply for example, UTM coordinates easting = 627594.0; northing = 4842250.0, Zone 17T for Toronto. Latitude: 43.654321; Longitude: -79.3837. The google earth view is:
    <img width="1081" alt="Screenshot 2024-11-13 at 9 57 45 pm" src="https://github.com/user-attachments/assets/c2ae2037-9965-4172-b178-54df684f155b">

## Results
The entire process and the results are as below.
  1. read point cloud ply file with open3d
  2. run RANSAC for road detection
  3. visualize road inliers and other outliers
     <img width="955" alt="Screenshot 2024-11-13 at 9 15 34 pm" src="https://github.com/user-attachments/assets/6ffa66dc-2c1b-42c6-b68a-5d30d00ff021">

  4. save inliers positions and colors into CSV
  5. visualize CSV
     <img width="947" alt="Screenshot 2024-11-13 at 10 14 36 pm" src="https://github.com/user-attachments/assets/782dc971-dcbd-4338-9490-fe6254503f0e">



## Acknowledgement
  * @inproceedings{tan2020toronto3d,
    title={{Toronto-3D}: A large-scale mobile lidar dataset for semantic segmentation of urban roadways},
    author={Tan, Weikai and Qin, Nannan and Ma, Lingfei and Li, Ying and Du, Jing and Cai, Guorong and Yang, Ke and Li, Jonathan},
    booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops},
    pages={202--203},
    year={2020}}
  * [pyRANSAC-3D](https://github.com/leomariga/pyRANSAC-3D)


