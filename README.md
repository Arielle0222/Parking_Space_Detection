## 🚙 Parking Space Detection Project using Image Processing and Object Recognition

**Team Name:** 기둥 뒤에 공간 있어요!  
**Project Duration:** August 20, 2024 - September 9, 2024  
**Team Members:**  
- **마석빈 (Team Lead):** Model building, visualization development, data preprocessing.  
- **김서희:** Data analysis, YOLO data preprocessing, model training, log management.  
- **박달님:** Data preprocessing, model training, image augmentation.  
- **이윤제:** Data preprocessing (excluding YOLO), model training, log management, image augmentation.

## 🔍 Project Overview
This project focuses on detecting parking spaces using both traditional image processing techniques and deep learning-based object recognition algorithms. Our objective is to develop an AI model for autonomous vehicles capable of accurately detecting and classifying parking spaces, driveable spaces, pedestrians, and vehicles.

## 🛠️ Model Implementation Summary

| **Model**    | **Backbone**         | **Purpose**                                                                 | **Training Details**                                                                 | **Performance**                                 | **Challenges**                                           |
|--------------|----------------------|-----------------------------------------------------------------------------|--------------------------------------------------------------------------------------|------------------------------------------------|----------------------------------------------------------|
| **Mask R-CNN** | ResNet-50 (ImageNet) | Object detection and instance segmentation for **Parking Spaces** and **Driveable Spaces** | - Classes: 2 (Parking Space, Driveable Space) <br> - Epochs: 10 <br> - Batch Size: 32 <br> - Optimizer: Adam (lr=0.001) | Achieved **82.7% AP** for parking space and driveable area detection | None                                                      |
| **YOLOv8**   | N/A                  | Enhance detection of smaller objects like **Pedestrians** and **Vehicles**  | - Classes: 2 (Person, Vehicle) <br> - Integrated with Mask R-CNN for better performance | Achieved **74.4% AP** with 4-class setup (Parking Space, Driveable Space, Person, Vehicle) | False positives (e.g., misclassifying trees or poles as people) |



## 💻 Technical Stack

### Programming Languages & Frameworks

<div align="left">
    <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=Python&logoColor=white" />
    <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=PyTorch&logoColor=white" />
    <img src="https://img.shields.io/badge/YOLO-00FFFF?style=flat&logo=YOLO&logoColor=black" />
</div>

### Computer Vision & GPU

<div align="left">
    <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=OpenCV&logoColor=white" />
    <img src="https://img.shields.io/badge/NVIDIA_CUDA-76B900?style=flat&logo=NVIDIA&logoColor=white" />
</div>

## 📼 Demo
👉 [Watch the demo video in here!](https://drive.google.com/drive/folders/1Vg_oa_r5s_gYFnLBLm-cYhLv_40ciIT6)

![YOLO Demo Image](yolo_demo_img.png)
![City Demo Image](city_demo_img.png)

---

## 📊 Dataset & References

- **AI Hub Parking Space Dataset:** [AI Hub Data Link](https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&dataSetSn=598)
- Reference 1: https://dacon.io/en/competitions/official/235672/codeshare/1795
- Reference 2: https://lyclyc52.github.io/SANeRF-HQ/
