# Berwick Academy Super Sleuths Ad Tracking

This project uses python 3, Selenium, pytest, and pyautogui to automate the clicking of banner ads on news websites, and captures the URL that the ad click navigates to.

The code and associated research were the result of work by a group of female high school students in southern Maine who became interested in the technologies and algorithms behind ad placement on news websites after hearing an [NPR interview on the topic](https://www.npr.org/2020/06/27/884213471/why-advertisers-wont-run-ads-on-black-lives-matter-content).

Your help with the project, either in the form of code improvements, new approaches, or data gathering, is much appreciated.  You can contact one of the group's coaches, Jeff Gunn, at jeff@loislab.org if you have questions.

## Prerequisites
Specific instructions will vary depending on the OS you're using.

**Python 3.x:** If your OS doesn't have python 3.x by default, you can visit https://www.python.org/ and go to 'downloads'.  Another option, which will also install various useful scientific tools and plugins, is to install the Anaconda distribution which is available for all major OSes.

**Selenium:** Once you have Python3 installed, you can install Selenium using the python package installer, pip.  Open a command prompt, and type 'pip install selenium'.

Next, you will need to install the Chrome webdriver (automatable browser):
- Determine what version of Chrome you have installed by opening Chrome and going to Help -> about Google Chrome and noting the version number
- Visit https://chromedriver.chromium.org/downloads and download the corresponding version of Chromium Webdriver
- The webdriver program will need to be located in your system path (the list of locations your computer knows to look for programs).  There may be a few steps involved, so google "add webdriver to system path" if you need help

**pytest:** Pytest will be installed with Anaconda if you went that route, otherwise you will need to add it by typing 'pip install pytest'.

**pyautogui:** As with the other components, you should be able to install this by typing 'pip install pyautogui'

To test these components, try the following:
- open python by going to a command prompt and typing 'python' (or 'python3' if you have both python versions 2 and 3 installed)
- type 'import selenium' and verify that you don't get an error
- type 'import pytest' and verify that you don't get an error
- type 'import pyautogui' and verify that you don't get an error
- if everything looks good, type 'quit()' to get back to your command prompt

At this point, you should be ready to download this repo and give it a try

## Tuning the code

You can probably tell from the comments, but you may have to change a couple of lines of code on your system:
- Pyautogui uses XY coordinates to click on banner ads, so depending on the size and resolution of your screen, this may change significantly.  Use trial and error to change the values in lines 31 & 32 until the mouse moves to the right location to hit the banner ad.
