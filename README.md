# PyLabRobot Tutorials BME590

### Installation

[Install Python=3.10](https://www.python.org/downloads/release/python-3110/)</br>
[Install Git](https://git-scm.com/downloads)</br>



### Installing PyLabRobot
From the terminal:</br>
`git clone https://github.com/PyLabRobot/pylabrobot.git` </br>
`cd pylabrobot`</br>
`pip install -e .[extras_visualizer]`</br>
`pip install libusb_package`</br>
`pip install websockets`</br>
`pip install jupyterlab`</br>
`cd ..`


### Setting up the virtual environment and dependencies
First, set up a virtual environment to prevent conflicts with any other projects
`pip install virtualenv`</br>
`virtualenv plr_env --python python3.10`</br>
`source plr_env/bin/activate`</br>
Now, install jupyterlab and uninstall existing libraries that can cause conflicts with the libraries we will be using. These conflicts mostly arise from the opentrons library, which requires certain dependencies with specific version numbers.
`pip install jupyterlab`</br>
`python3 -m pip uninstall -y jupyter ipython jupyter_core ipykernel jupyter-client jupyter-console jupyterlab_pygments qtconsole notebook nbconvert nbformat nbclassic nbclient jupyterlab-widgets jupyter-events jupyter-server jupyter-server-terminals`</br>
`pip install ipykernel==6.29.3`</br>
`pip install ipython==8.25.0`</br>
`pip install opentrons`</br>


### Opening the tutorials notebook
`git clone https://github.com/stefangolas/PyLabRobot_Tutorials_BME590.git`</br>
`cd PyLabRobot_Tutorials_BME590`</br>
`jupyter lab`</br>


## Notebook
 The last command should have opened the Jupyter Lab notebook shown below. This is an example script that gives an overview of PyLabRobot's capabilities.
 There are other scripts that delve into specific topics such as `DataSimulations` that you can access from the same directory. Feel free to change the scripts
 to get a sense of what PyLabRobot can do.

 ![image](Readme_Images/screenshot.png)
