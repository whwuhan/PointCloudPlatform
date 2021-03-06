[TOC]
# PointCloudPlatform
## 1.简介  
这是一个macOS下的，基于[PCL](https://pointclouds.org/)的点云处理平台，支持.obj .ply .pcd文件。  
所有的源代码都可以在/PointCloudPlatform/src下查看。  
macOS可以用Xcode打开/pcp.xcodeproj查看源代码。  

---
## 2.macOS下启动程序   
```
% cd your_path/PointCloudPlatform/Build/Products/Debug  
% ./pcp  
```
![./pcp](image/QQ20200630-123927@2x.png)  

---
## 3.IO
### 3.1 读取点云数据并显示点云数据  
```  
[Point Cloud Platform:]read your_point_cloud_data_path
[Point Cloud Platform:]show
```
![read](image/QQ20200630-145641@2x.png)  
![point_cloud](image/tree_point_cloud_1.png)  

---
### 3.2.存储处理后的点云  
```
[Point Cloud Platform:]write your_point_cloud_save_path
```
![write](image/QQ20200701-201648@2x.png)  

---
## 4 .归一化点云并显示  
```
[Point Cloud Platform:]read your_point_cloud_data_path
[Point Cloud Platform:]nor
[Point Cloud Platform:]show
```

---
## 5.点云重建  
### 5.1泊松重建
```
[Point Cloud Platform:]read your_point_cloud_data_path
[Point Cloud Platform:]pos
```
![pos](image/QQ20200702-212511.png)  
![pos_result](image/tree_mesh_pos_1.png)  

---
### 5.2.贪婪投影三角重建  
```
[Point Cloud Platform:]read your_point_cloud_data_path
[Point Cloud Platform:]gp3
```
![gp3](image/QQ20200702-185753.png)  
![gp3_result](image/tree_mesh_gp3_1.png)  