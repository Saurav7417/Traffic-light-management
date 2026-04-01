🚦 AI-Based Traffic Management System

📌 Overview

This project is an AI-powered Traffic Management System built using Python, OpenCV, and NumPy.
It dynamically controls traffic signals based on real-time vehicle density, improving traffic flow and reducing congestion.

The system captures images/videos, processes them to estimate traffic density, and automatically adjusts signal timings using intelligent algorithms.

🚀 Features
📷 Real-time image/video processing using OpenCV
🚗 Vehicle density estimation
🧠 Adaptive traffic signal control using algorithms
⏱ Dynamic green signal timing based on traffic load
📊 Uses NumPy for efficient calculations
🔄 Simulation of multi-lane traffic system
⚡ Supports multiple traffic control strategies

🛠️ Technologies Used
Python
OpenCV
NumPy
Deque (collections)
Time module

⚙️ How It Works
The system captures traffic data (image/video input).
OpenCV processes frames to detect vehicles.
NumPy calculates vehicle density.
Based on density:
Green signal time is calculated.
Priority is given to lanes with more vehicles.
Traffic signals rotate dynamically.

🧠 Algorithms Used
1. Linear Formula
green_time = 15 + (vehicles * 2) + (wait_time // 10)
2. Weighted Priority
priority = (vehicles * 0.6) + (wait_time * 0.4)
green_time = 15 + (priority * 1.5)
3. Adaptive Threshold (Implemented)
Vehicles < 5 → 20 sec
Vehicles < 15 → 30 sec
Vehicles ≥ 15 → 45 sec
✔ Ensures optimal traffic flow and avoids starvation of lanes

▶️ How to Run
git clone https://github.com/your-username/traffic-management-system.git
cd traffic-management-system
python main.py

📷 Sample Workflow
Input: Vehicle count per lane
Output: Dynamic signal switching with calculated green time

📈 Future Improvements
Integrate YOLO or Deep Learning models for accurate vehicle detection
Add GUI Dashboard
Deploy on IoT-based traffic signals
Real-time API integration with traffic cameras
Use Reinforcement Learning for smarter decision making

🤝 Contribution
Feel free to fork this repo and improve the system!

📬 Contact
Saurav Kumar
BTech CSE Student
