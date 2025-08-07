# Object Tracking using OpenCV in Python

A Python-based project demonstrating real-time object detection and centroid-based tracking using OpenCV.

## 🧠 Overview

This repository implements a simple object tracking pipeline using OpenCV and centroid tracking logic. Each detected object is assigned a unique ID and tracked across frames by comparing object centroids. When objects disappear or reappear, IDs are updated accordingly.

## 📁 Project Structure

```

/
├── 49_Object Tracking and Detection.ipynb                  # Main tracking script
├── requirements.txt         # Python dependencies
└── README.md

````

## 🚀 Features

- Centroid-based object tracking
- Unique ID assignment per object
- Removal of lost objects from memory
- Bounding box and ID visualization in real-time

## 🛠️ Installation & Usage

1. **Clone the repository:**

```bash
git clone https://github.com/HafsaNoorMuhammad26/Object-Tracking-using-OpenCV-Python.git
cd Object-Tracking-using-OpenCV-Python
````

2. **Install required libraries:**

```bash
pip install -r requirements.txt
```

3. **Run the tracker:**

```bash
python 49_Object Tracking and Detection.py
```

## 🧠 How It Works

1. Detect objects or manually select them using OpenCV.
2. Calculate the centroid `(cx, cy)` of each bounding box.
3. Match new centroids to previous ones by Euclidean distance.
4. Assign or update object IDs.
5. Track objects in real-time with updated bounding boxes and labels.

## 📦 Dependencies

```
opencv-python
numpy
imutils
```

Install them via:

```bash
pip install -r requirements.txt
```

## 📈 Tracker Options in OpenCV

You can change the tracker algorithm (like `KCF`, `CSRT`, `MOSSE`) in the code:

```python
cv2.TrackerCSRT_create()
cv2.TrackerKCF_create()
cv2.TrackerMOSSE_create()
```

## ✅ Future Improvements

* Integration with YOLOv8 for improved detection
* Tracking multiple objects with DeepSORT
* GUI for easier interaction
* Save tracking logs to file

## 📜 License

This project is licensed under the MIT License – feel free to use and modify it.

## 👩‍💻 Author

**Hafsa Noor Muhammad**
🎓 BS Software Engineering Student | 💼 Junior Data Analyst
🔗 [GitHub Profile](https://github.com/HafsaNoorMuhammad26)
🔗 [LinkedIn](https://www.linkedin.com/in/hafsa-noor-muhammad-67b96331a/)

---

Feel free to ⭐ the repo if you find it useful!

```
