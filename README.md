Getting Started with Crazyflie: Takeoff and Landing via Python

This tutorial walks you through how to:

- Set up your system from scratch  
- Install the necessary software  
- Connect your Crazyflie drone  
- Run a Python script that makes the drone take off, hover, and land smoothly  

What You’ll Need

- Crazyflie 2.1 nano quadcopter  
- Crazyradio PA USB dongle  
- Charged battery in the drone  
- A macOS or Linux laptop  
- A safe open area to fly the drone  

Step 1: Install Python 3

macOS:

brew install python

Ubuntu:

sudo apt update  
sudo apt install python3 python3-pip

Verify installation:

python3 --version  
pip3 --version

Step 2: Set Up a Virtual Environment

Create and activate a virtual environment:

python3 -m venv venv  
source venv/bin/activate

Install the Crazyflie Python library:

pip install cflib

Step 3: Set Up the Flight Script

Create a folder and move into it:

mkdir -p ~/crazyflie-flight  
cd ~/crazyflie-flight

Download the cf_up_min.py script:

1. Open the cf_up_min.py file in this repository  
2. Click Raw  
3. Right-click and select "Save As…"  
4. Save it into your ~/crazyflie-flight folder  

Step 4: Power On and Connect the Drone

1. Plug in the Crazyradio PA USB dongle  
2. Connect the battery to the Crazyflie (it powers on automatically)  
3. Wait for LEDs to blink, indicating the drone is ready  
4. Place the drone on a flat surface  

Step 5: Run the Flight Script

Make sure you're in the right folder and your virtual environment is active:

cd ~/crazyflie-flight  
source ../venv/bin/activate  
python3 cf_up_min.py

What the Drone Will Do

- Ramp up motors gradually  
- Take off and climb briefly  
- Hover in place  
- Land smoothly  
- Shut off motors completely
