ARJewelBox - Virtual Jewelry Try-On System
Author: Pranesh Prabaharan K
ARJewelBox is an interactive software application that allows users to try on jewelry virtually using Augmented Reality (AR) technology. By utilizing a camera and screen, users can see themselves wearing various jewelry pieces in real time — without needing to handle the actual products.
This system is ideal for jewelry retailers and e-commerce platforms seeking to enhance their customers’ online shopping experience and boost engagement and sales.
🪄 Credits & Usage
You may use this source code for educational purposes as long as you provide proper credit to the author — Pranesh Prabaharan K.
If you find this project useful, please give a star ⭐ and follow for more projects.
📸 Screenshots
⚙️ How to Use
This project is built using Python and OpenCV, and tested on Python 3.9.13 with the dependencies listed below.
Step 1: Install Dependencies
pip install numpy==1.24.3
pip install opencv-python==4.7.0.72
Step 2: Run the Application
If you prefer not to install Python or dependencies manually, simply go to the dist directory and
download the executable version — Try-ARJewelBox.exe — and run it directly.
💡 Functionalities
On launching the application, a loading screen appears.
Once loaded:
If run from the executable file → the default webcam opens.
If run directly from source → a test video (provided copyright-free).
The video source can be changed in the code as explained below.
Keyboard Controls
Key	Action
ESC	Quit the application
P/p	Show previous jewelry
N/n	Show next jewelry
S/s	Save / Capture the image
🧩 Using the Source Code
1. Select Video Source
Modify the following lines in main.py:
VID_SOURCE = "USB_CAM"
# VID_SOURCE = "FILE"
# VID_SOURCE = "RTSP"
2. Update Settings
To use FILE or RTSP, update paths in
assets/configs/settings.json:
{
    "USB_CAM": 0,
    "FILE": "assets/test_video/test.mp4",
    "RTSP": "rtsp://192.168.1.1:8080/out.h264"
}
💍 Adding New Jewelry
Download a jewelry image with a transparent background.
Place it in the assets/jewellery folder.
Open the assets/configs/jewellery.json file and add the new entry:
"jewel5": {
  "path": "assets/jewellery/5.png",
  "x": 0,
  "y": 0,
  "dw": 1,
  "dh": 1
}
Adjust x, y, dw, and dh values through hit-and-trial to achieve the perfect fit.
Re-run the program to see and try your newly added jewelry!
🧾 License
This project is released under the MIT License.
© 2025 Pranesh Prabaharan K. All rights reserved.