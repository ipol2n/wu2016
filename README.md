# ATDD using Robot Framework and TDD with Python

## Install Python 3.4.4
https://www.python.org/downloads/

Note:

- For Windows, you have to add Python installation path to the Environment Variable in the next step

### Setup PATH environment variable for Windows only
1. Press "Windows + Pause" button
2. Click "Advance System Settings"
3. Click "Environment Variables"
4. Edit value of `Path` variable, append Python installation path at the end

### Verify Installed Python
1. Open command prompt/terminal
2. Run `python --version`
```bash
python --version
Python 3.4.4
```
You should see the version of installed Python on your machine

## Install PIP

### Windows
```bash
python -m pip install --upgrade pip
python -m pip --version
pip 9.0.1 from C:\Python34\lib\site-packages (python 3.4)
```
You should see the version of installed PIP on your machine

### Mac OS/Linux
```bash
wget https://bootstrap.pypa.io/get-pip.py && sudo python get-pip.py
pip --version
pip 8.1.2 from /env/lib/python3.5/site-packages (python 3.5)
```
You should see the version of installed PIP on your machine


## Install Virtualenv

### Windows
```bash
python -m pip install virtualenv
```

### MacOS/Linux
```bash
pip install virtualenv
```

## Create Project and setup environment

1. Create directoty at "/home/my-robot" or "c:\my-robot" for Windows

2. Goto project directory and init Git repository

3. Create our development environment and activate virtualenv

Windows
```bash
python -m virtualenv env
env\scripts\activate
```

MacOS/Linux
```bash
virtualenv env
. env/bin/activate
```

The result should be
```bash
Installing setuptools, pip, wheel...done
```

## Install dependencies

Create "requirements.txt" and add the following lines

```text
robotframework
robotframework-selenium2library
```
Run `pip install -r requirements.txt`

### Alternate installation steps
1. Run `pip install robotframework`
2. Run `pip install robotframework-selenium2library`

## Robot Framework verification
Run `robot --version`
```bash
robot --version
Robot Framework 3.0 (Python 3.5.1 on darwin)
```
You should see the version of installed Robot Framework on your machine

## Download Browsers drivers
### Chrome driver
https://sites.google.com/a/chromium.org/chromedriver/
### Internet Explorer
http://www.seleniumhq.org/download/

