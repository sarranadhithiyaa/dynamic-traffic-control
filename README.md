# dynamic-traffic-control
### 🚗🚦 **Project Description: YOLO + CNN Vehicle Detection & Classification** 🚀  

This project combines **YOLO (You Only Look Once) object detection** and a **CNN-based classification model** to identify and classify vehicles in an image. The main components are:

### 🔍 **1. YOLO for Vehicle Detection**  
✅ Detects objects in the image.  
✅ Filters out detected objects to keep only vehicles (**cars, trucks, buses, motorbikes**).  
✅ Uses **Non-Maximum Suppression (NMS)** to remove duplicate detections.  

### 🎯 **2. CNN for Vehicle Classification**  
🖼️ Crops detected vehicle regions.  
📏 Preprocesses the image (**resizing, normalization**).  
🤖 Uses a pre-trained **CNN model** to classify the vehicle into one of the categories:  
   - 🚖 **Auto Rickshaw**  
   - 🏍️ **Bike**  
   - 🚗 **Car**  
   - 🏍️ **Motorcycle**  
   - ✈️ **Plane**  
   - 🚢 **Ship**  
   - 🚆 **Train**  


🎨 4. Result Visualization  
📦 Draws bounding boxes around detected vehicles.  
📝 Displays vehicle labels & confidence scores.  
📊 Shows vehicle count & green light duration on the image.  

---
dataset to train cnn model
import kagglehub

# Download latest version
path = kagglehub.dataset_download("mohamedmaher5/vehicle-classification")

print("Path to dataset files:", path)

