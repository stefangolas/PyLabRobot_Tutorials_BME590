# PyLabRobot Tutorials BME590

### Required software installs

[Install Python=>3.10](https://www.python.org/downloads/release/python-3110/) </br>
[Install Git](https://git-scm.com/downloads)</br>


### Setting up the virtual environment and dependencies
1. First, set up a virtual environment to prevent conflicts with any other projects
```bash
pip install virtualenv
virtualenv plr_env --python python3.11
source plr_env/bin/activate
```



### Installing PyLabRobot
From the terminal:</br>
```bash
git clone https://github.com/PyLabRobot/pylabrobot.git
cd pylabrobot
pip install -e '.[visualizer]'
pip install libusb_package
pip install websockets
cd ..
```

Now, install jupyterlab and all the other dependencies. Make sure to pip install opentrons with `--no-deps`.
```bash
pip install jupyterlab
pip install pylibftdi
pip install aionotify==0.3.1
pip install pydantic==1.10.9
pip install ipykernel==6.29.3
pip install ipython==8.25.0
pip install pyserial
pip install numpy
pip install opentrons --no-deps
pip install opentrons_shared_data --no-deps
```

### Opening the tutorials notebook
```bash
git clone https://github.com/stefangolas/PyLabRobot_Tutorials_BME590.git
cd PyLabRobot_Tutorials_BME590
jupyter lab
```

## Notebook
 The last command should have opened the Jupyter Lab notebook shown below. This is an example script that gives an overview of PyLabRobot's capabilities.
 There are other scripts that delve into specific topics such as `DataSimulations` that you can access from the same directory. Feel free to change the scripts
 to get a sense of what PyLabRobot can do.

 ![image](Readme_Images/screenshot.png)
