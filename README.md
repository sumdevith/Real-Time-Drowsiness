
🚗 Real-Time Drowsiness Detection System
<div align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=Drowsiness%20Detection&fontSize=50&fontAlignY=35&animation=twinkling" width="100%"/> </div><div align="center"> <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=00FF00&center=true&vCenter=true&width=435&lines=Real-Time+Detection;95%25+Accuracy;Deep+Learning;Computer+Vision" alt="Typing SVG" /> </div>
<div align="center"> <img src="https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white"> <img src="https://img.shields.io/badge/TensorFlow-2.0-orange?style=for-the-badge&logo=tensorflow&logoColor=white"> <img src="https://img.shields.io/badge/OpenCV-4.5-green?style=for-the-badge&logo=opencv&logoColor=white"> <img src="https://img.shields.io/badge/Accuracy-95%25-brightgreen?style=for-the-badge"> <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"> </div>
<!-- Animated Divider --><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
📌 Overview
<table> <tr> <td width="60%">
🎯 Project Description
An intelligent real-time driver drowsiness detection system using Deep Learning & Computer Vision. Monitors eye states through webcam and triggers alerts to prevent accidents caused by driver fatigue.

✨ Key Highlights
✅ 95%+ detection accuracy

✅ Real-time processing (15-20 FPS)

✅ 84,898 training images

✅ Works in various lighting conditions

</td> <td width="40%" align="center"><!-- Animated Car GIF --><img src="https://media.giphy.com/media/l4EpblDY4msVtQk2Q/giphy.gif" width="250"></td> </tr> </table><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
🎯 Features
<div align="center"> <table> <tr> <td align="center" width="200"> <img src="https://img.icons8.com/fluency/96/000000/face-id.png"/> <br> <b>Face Detection</b> <br> <small>Haar Cascade</small> </td> <td align="center" width="200"> <img src="https://img.icons8.com/fluency/96/000000/artificial-intelligence.png"/> <br> <b>CNN Model</b> <br> <small>11.2M Parameters</small> </td> <td align="center" width="200"> <img src="https://img.icons8.com/fluency/96/000000/alarm.png"/> <br> <b>Real-time Alert</b> <br> <small>Visual Warning</small> </td> <td align="center" width="200"> <img src="https://img.icons8.com/fluency/96/000000/visible.png"/> <br> <b>Eye Tracking</b> <br> <small>Open/Closed</small> </td> </tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
📁 Project Structure
<pre> 📦 <b>drowsiness-detection</b> ├── 📂 <b>DataClean</b> │ ├── 📂 open <span style="color:green"># 42,952 open eye images</span> │ └── 📂 close <span style="color:red"># 41,946 closed eye images</span> ├── 📓 <b>clean_data.ipynb</b> <span style="color:gray"># Dataset preprocessing</span> ├── 📓 <b>real_time_drowsiness.ipynb</b> <span style="color:gray"># Training notebook</span> ├── 🐍 <b>demo.py</b> <span style="color:gray"># Detection script</span> ├── 🧠 <b>drowsiness_eye_model.h5</b> <span style="color:gray"># Trained model</span> ├── 📦 <b>requirements.txt</b> <span style="color:gray"># Dependencies</span> └── 📖 <b>README.md</b> <span style="color:gray"># Documentation</span> </pre><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
🗂️ Dataset: MRL Eye Dataset
<div align="center"> <table border="1" cellpadding="10" cellspacing="0"> <tr> <th colspan="3" bgcolor="#363636">📊 Dataset Statistics</th> </tr> <tr> <th>Category</th> <th>Count</th> <th>Percentage</th> </tr> <tr> <td><span style="color:green">✅ Open Eyes</span></td> <td align="center"><b>42,952</b></td> <td align="center"><progress value="42952" max="84898" style="width:100px"></progress> 50.6%</td> </tr> <tr> <td><span style="color:red">⚠️ Closed Eyes</span></td> <td align="center"><b>41,946</b></td> <td align="center"><progress value="41946" max="84898" style="width:100px"></progress> 49.4%</td> </tr> <tr> <td><b>TOTAL</b></td> <td align="center"><b>84,898</b></td> <td align="center">100%</td> </tr> </table> </div>
🎭 Dataset Features
<div align="center"> <table> <tr> <td align="center">☀️</td> <td>Various lighting conditions</td> </tr> <tr> <td align="center">👓</td> <td>With/without glasses</td> </tr> <tr> <td align="center">👤</td> <td>Multiple subjects</td> </tr> <tr> <td align="center">🌍</td> <td>Different ethnicities</td> </tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
🧠 Model Architecture
<div align="center"> <table border="1" cellpadding="8" cellspacing="0" style="border-collapse: collapse; width: 80%;"> <tr> <th colspan="3" bgcolor="#2c3e50"><span style="color:white">Sequential Model</span></th> </tr> <tr> <th>Layer</th> <th>Output Shape</th> <th>Parameters</th> </tr> <tr><td>Rescaling</td><td>(224,224,1)</td><td align="right">0</td></tr> <tr><td>Conv2D (32)</td><td>(222,222,32)</td><td align="right">320</td></tr> <tr><td>MaxPooling2D</td><td>(111,111,32)</td><td align="right">0</td></tr> <tr><td>Conv2D (64)</td><td>(109,109,64)</td><td align="right">18,496</td></tr> <tr><td>MaxPooling2D</td><td>(54,54,64)</td><td align="right">0</td></tr> <tr><td>Conv2D (128)</td><td>(52,52,128)</td><td align="right">73,856</td></tr> <tr><td>MaxPooling2D</td><td>(26,26,128)</td><td align="right">0</td></tr> <tr><td>Flatten</td><td>(86,528)</td><td align="right">0</td></tr> <tr><td>Dense (128)</td><td>(128)</td><td align="right">11,075,712</td></tr> <tr><td>Dropout (0.5)</td><td>(128)</td><td align="right">0</td></tr> <tr><td>Dense (1)</td><td>(1)</td><td align="right">129</td></tr> <tr> <td colspan="2"><b>Total Parameters</b></td> <td align="right"><b>11,168,513</b></td> </tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
📊 Results
<div align="center"> <table border="1" cellpadding="15" cellspacing="0" style="border-collapse: collapse; width: 60%;"> <tr> <th colspan="2" bgcolor="#27ae60"><span style="color:white">🎯 Performance Metrics</span></th> </tr> <tr> <td><b>Test Accuracy</b></td> <td align="center"><span style="color:#27ae60; font-size:20px;"><b>95.29%</b></span></td> </tr> <tr> <td><b>Test Loss</b></td> <td align="center"><span style="color:#e74c3c;"><b>0.1295</b></span></td> </tr> <tr> <td><b>Training Time</b></td> <td align="center">~20 minutes (CPU)</td> </tr> <tr> <td><b>Inference Speed</b></td> <td align="center">15-20 FPS</td> </tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
🚀 How It Works
<div align="center"></div><div align="center"> <table border="0" cellpadding="20" style="width:80%; background:#0a1929; border-radius:15px;"> <tr align="center"> <td><img src="https://img.icons8.com/fluency/96/000000/video-call.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/arrow.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/face-scan.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/arrow.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/iris-scan.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/arrow.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/brain.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/arrow.png"/></td> <td><img src="https://img.icons8.com/fluency/96/000000/alarm-bell.png"/></td> </tr> <tr align="center"> <td><b>Capture</b></td> <td></td> <td><b>Detect</b></td> <td></td> <td><b>Extract</b></td> <td></td> <td><b>Classify</b></td> <td></td> <td><b>Alert</b></td> </tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
💻 Installation
<div align="center"> <div style="background:#0d1117; border-radius:10px; padding:20px; text-align:left; font-family:monospace;">
bash
# Clone repository
https://github.com/yourusername/drowsiness-detection.git
cd drowsiness-detection

# Install dependencies
pip install -r requirements.txt
</div> </div>
📦 Dependencies
<div align="center"> <table border="1" cellpadding="10" style="border-collapse: collapse;"> <tr> <th>Package</th> <th>Version</th> </tr> <tr><td>opencv-python</td><td>≥4.5.0</td></tr> <tr><td>tensorflow</td><td>≥2.0.0</td></tr> <tr><td>numpy</td><td>≥1.19.0</td></tr> <tr><td>matplotlib</td><td>≥3.3.0</td></tr> <tr><td>scikit-learn</td><td>≥0.24.0</td></tr> <tr><td>jupyter</td><td>≥1.0.0</td></tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
📝 Usage
🚀 Quick Start
<div align="center"> <table border="0" style="width:90%; background:#1e1e2f; border-radius:15px;"> <tr> <td align="center" width="33%"> <h3>1️⃣</h3> <img src="https://img.icons8.com/fluency/96/000000/database.png"/> <br> <b>Prepare Dataset</b> <br> <code>jupyter notebook clean_data.ipynb</code> </td> <td align="center" width="33%"> <h3>2️⃣</h3> <img src="https://img.icons8.com/fluency/96/000000/training.png"/> <br> <b>Train Model</b> <br> <code>jupyter notebook real_time_drowsiness.ipynb</code> </td> <td align="center" width="33%"> <h3>3️⃣</h3> <img src="https://img.icons8.com/fluency/96/000000/video-playlist.png"/> <br> <b>Run Detection</b> <br> <code>python demo.py</code> </td> </tr> </table> </div>
🎮 Controls
<div align="center"> <kbd>q</kbd> - Quit &nbsp;&nbsp;&nbsp; <kbd>Space</kbd> - Pause &nbsp;&nbsp;&nbsp; <kbd>s</kbd> - Screenshot </div>
🎨 Visual Indicators
<div align="center"> <table border="1" style="border-collapse: collapse;"> <tr> <td><span style="color:green">🟢 Green Box</span></td> <td>Eyes detected & open</td> </tr> <tr> <td><span style="color:yellow">🟡 Yellow Box</span></td> <td>Eyes detected & closed</td> </tr> <tr> <td><span style="color:red">🔴 Red Alert</span></td> <td>Drowsy! (20+ frames closed)</td> </tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
⚙️ Configuration
<div align="center"> <div style="background:#0d1117; border-radius:10px; padding:20px; text-align:left;">
python
# Adjust these parameters in demo.py
DROWSY_THRESHOLD = 20     # Frames before alert
IMG_SIZE = 224            # Input image size
CAMERA_INDEX = 0          # 0=built-in, 1=external
</div> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
📈 Future Improvements
<div align="center"> <table border="0" style="width:80%;"> <tr> <td align="left"> <ul style="list-style-type: none;"> <li>✅ <input type="checkbox" disabled> Audio Alarm</li> <li>✅ <input type="checkbox" disabled> Night Vision</li> <li>✅ <input type="checkbox" disabled> Mobile App</li> <li>✅ <input type="checkbox" disabled> Vehicle Integration</li> <li>✅ <input type="checkbox" disabled> Data Logging</li> <li>✅ <input type="checkbox" disabled> Head Pose Estimation</li> </ul> </td> </tr> </table> </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
⚠️ Important Notes
<div style="background:#fff3cd; border-left:6px solid #ffc107; padding:15px; border-radius:5px;"> <h4>📁 Large Files Not Included</h4> <ul> <li><code>drowsiness_eye_model.h5</code> (134MB) - Download from <a href="#">Google Drive</a></li> <li><code>mrlEyes_2018_01/</code> (Several GB) - Download from <a href="http://mrl.cs.vsb.cz/eyedataset">official source</a>>official source</a></li> </ul> </div>
<div style="background:#d4edda; border-left:6px solid #28a745; padding:15px; border-radius:5px;"> <h4>📥 Getting the Model</h4> <b>Option 1:</b> Train your own using <code>real_time_drowsiness.ipynb</code><br> <b>Option 2:</b> Download pre-trained model from <a href="#">link</a> (coming soon) </div><img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
🙏 Acknowledgments
<div align="center"> <table style="border:none;"> <tr> <td align="center"><img src="https://img.icons8.com/fluency/48/000000/hearts.png"/></td> <td><b>MRL Eye Dataset</b> creators</td> </tr> <tr> <td align="center"><img src="https://img.icons8.com/fluency/48/000000/opencv.png"/></td> <td><b>OpenCV</b> community</td> </tr> <tr> <td align="center"><img src="https://img.icons8.com/fluency/48/000000/tensorflow.png"/></td> <td><b>TensorFlow</b> team</td> </tr> </table> </div>
<div align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=150&section=footer&text=Stay%20Safe%20on%20the%20Road&fontSize=30&fontAlignY=70" width="100%"/> <br> <img src="https://profile-counter.glitch.me/drowsiness-detection/count.svg" alt="Visitor Count"> <br> <p>⭐ <b>Star this repository if you find it useful!</b> ⭐</p> <p>Built with ❤️ for road safety</p> </div>
