# Getting-Started-with-Crazyflie

Getting Started with Crazyflie: Takeoff and Landing via Python

This tutorial shows you how to: 
1. Set up your system from scratch
2. Install the necessary software
3. Connect your Crazyflie drone
4. Run a script that makes the drone take off, hover and land smoothly

What You Need
- Crazyflie 2.1 nano quadcopter
- Crazyradio PA USB dongle
- Charged battery in drone
- A laptop running macOS or Linux
- A safe open area to fly 

Step 1: Install Python 3
- Open your terminal and install Python 3:  <img width="1237" height="170" alt="Screenshot 2025-11-03 at 4 24 55 PM" src="https://github.com/user-attachments/assets/6b3f327c-a11f-4b9a-a998-93f590db8f51" />


- Verify that Python is installed <img width="870" height="64" alt="image" src="https://github.com/user-attachments/assets/2fb4b619-0fdb-475e-b483-25b47d59635b" />



Step 2: Create a Virtual Environment
- This will help keep your project clean and organized.
- Create and activate a virtual environment: <img width="1063" height="117" alt="image" src="https://github.com/user-attachments/assets/d910399d-49c1-43a8-b8e2-c447053896af" />
- Install the Crazyflie Python Library  <img width="1171" height="84" alt="image" src="https://github.com/user-attachments/assets/b2cea11a-6f2d-4e04-90eb-eefe630c45c9" />
This gives you access to the cflib API to talk to the drone

Step 3: Set Up the Flight Script
- Create a folder and write a script: <img width="710" height="98" alt="image" src="https://github.com/user-attachments/assets/20dcfc28-6b77-4cfb-8402-8bfbf0da71f3" />
- Open the cf_up_min.py file in this repo
- Click Raw, then save the page as cf_up_min.py
- Move the file into a folder like ~/crazyflie-flight

Step 3: Power On and Connect the Drone: 
1. Plug the Crazyradio PA into your computer
2. Connect the battery to the Crazyflie, it will power on automatically.
3. Wait for LEDs to blink, then place the drone on a flat surface

Step 4: Run the Script 
1. Make sure that your virtual environment is active and run the script: <img width="1230" height="102" alt="image" src="https://github.com/user-attachments/assets/a75ed261-b27f-4c65-85f8-fc45854cf539" />
The drone will:
- Ramp up motors
- Take off and climb briefly
- Hover
- Land using a cosine easing curve
- Shut off motors fully 
