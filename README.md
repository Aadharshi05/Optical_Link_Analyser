# Optical_Link_Analyser

📡 Optical Link Design & Analysis Dashboard:
      A modern, single-file web application for designing and analyzing optical fiber communication links. This dashboard provides real-time calculations, visualizations, and system validation in a sleek, professional UI.

🚀 Features:

🎛️ Interactive Sidebar Inputs:

Power Budget Parameters,
Transmit Power (dBm),
Fiber Length (km),
Attenuation (dB/km),
Number of Splices (0.1 dB each),
Number of Connectors (0.5 dB each),
System Margin (default: 3 dB),
Dispersion Parameters,
Bit Rate (Gbps),
Dispersion Coefficient (ps/nm·km)

⚡ Real-Time Calculations:

All values update instantly with no page reload:
Total Link Loss

TotalLoss = (L × α) + (Ns × 0.1) + (Nc × 0.5) + Margin

Received Power

Prx = Ptx - TotalLoss

Dispersion Check

Pulse broadening vs. bit period:

T = 1 / BitRate

Determines if the system is bandwidth-limited

📊 Visual Dashboard:

Dynamic Line Chart,
Signal Power (dBm) vs Distance (km),
Built using Chart.js (CDN),
Status Cards,
Total Attenuation (dB),
Power at Receiver (dBm),
Dispersion Limit (ps),
System Verdict Badge


🟢 LINK SUCCESS 

Power > -30 dBm AND dispersion within limits

🔴 SIGNAL CRITICAL

Power too low

🟠 BANDWIDTH LIMITED

Dispersion exceeds bit period

🎨 UI & Design:

Dark and Light theme options provided.
Theme: Rose Gold & Charcoal,
Rose Gold: #B76E79,
White: #FFFFFF,
Charcoal: #2C3E50,
Design Style,
Glassmorphism effects,
Smooth transitions,
Rounded corners (16px),
Sidebar → Main Panel layout

📦 Tech Stack:

HTML5,
CSS3 (Glassmorphism + Flexbox/Grid),
Vanilla JavaScript,
Chart.js (via CDN)

🧠 How It Works:

User inputs parameters in the sidebar
JavaScript listens for input changes

Calculations update instantly:

Link loss,
Received power,
Dispersion condition,
Chart and UI components re-render dynamically,
System verdict updates in real-time

📈 Example Use Case:

A fiber technician can:

Estimate signal degradation over distance,
Check if received power is sufficient,
Validate whether dispersion will affect transmission,
Make quick decisions in the field

🎯 Project Goal:

To simulate a real-world optical link analysis tool with:
Instant feedback,
Professional UI,
Engineering accuracy

📜 License:

This project is for academic and educational use.
