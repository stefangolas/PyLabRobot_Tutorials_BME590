# PyLabRobot Tutorials BME590

### Required software installs

[Install Python=3.10](https://www.python.org/downloads/release/python-3110/) (you need to specifically have version 3.10 to use the opentrons library)</br>
[Install Git](https://git-scm.com/downloads)</br>



### Installing PyLabRobot
From the terminal:</br>
```bash
git clone https://github.com/PyLabRobot/pylabrobot.git
cd pylabrobot
pip install -e .[extras_visualizer]
pip install libusb_package
pip install websockets
cd ..
```

### Setting up the virtual environment and dependencies
1. First, set up a virtual environment to prevent conflicts with any other projects
```bash
pip install virtualenv
virtualenv plr_env --python python3.10
source plr_env/bin/activate
```

2. Now, install jupyterlab and uninstall existing libraries that can cause conflicts with the libraries we will be using. These conflicts mostly arise from the opentrons library, which requires certain dependencies with specific version numbers.
```bash
pip install jupyterlab
python3 -m pip uninstall -y jupyter ipython jupyter_core ipykernel jupyter-client jupyter-console jupyterlab_pygments qtconsole notebook nbconvert nbformat nbclassic nbclient jupyterlab-widgets jupyter-events jupyter-server jupyter-server-terminals
pip install ipykernel==6.29.3
pip install ipython==8.25.0
pip install opentrons
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
