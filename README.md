# PyLabRobot Tutorials BME590

## Installation

[Install Python](https://www.python.org/downloads/release/python-3110/)</br>
[Install Git](https://git-scm.com/downloads)</br>


From the terminal:</br>
`git clone https://github.com/PyLabRobot/pylabrobot.git` </br>
`cd pylabrobot`</br>
`pip install -e .[extras_visualizer]`</br>
`pip install libusb_package`</br>
`pip install websockets`</br>
`pip install jupyterlab`</br>
`git clone https://github.com/stefangolas/PyLabRobot_Tutorials_BME590.git`</br>
`cd PyLabRobot_Tutorials_BME590`</br>
`jupyter lab`</br>

### Installation notes

* It's possible you already have a version of some of the dependencies that get installed alongside. If you are worried about conflicts with existing packages, you can use a virtual environment. [How to Use Python Virtual Environments](https://realpython.com/python-virtual-environments-a-primer/).

* You can use standard Jupyter Notebooks, but Jupyter Lab has a file system feature that is very convenient for navigating the repository.

* If you get an error that says `pip not recognized` on Windows, you just have to add your Python installation path to your environment variables. [Stack Overflow: pip is not recognized as an internal or external command](https://stackoverflow.com/questions/23708898/pip-is-not-recognized-as-an-internal-or-external-command).


This will install PyLabRobot in such a way that if you change the source code you just cloned, those changes will be reflected in your working version of the library when you import it into Python. This means that you can break your own installation of PLR, but you can always re-clone from the main repo to start over.

## Notebook
 The last command should have opened the Jupyter Lab notebook shown below. This is an example script that gives an overview of PyLabRobot's capabilities.
 There are other scripts that delve into specific topics such as `DataSimulations` that you can access from the same directory. Feel free to change the scripts
 to get a sense of what PyLabRobot can do.

 ![image](Readme_Images/screenshot.png)
