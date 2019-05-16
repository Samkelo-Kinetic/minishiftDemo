# Vula Mobile Functional Testing
![|Solid](http://www.globalafricanbusinessawards.com/wp-content/uploads/2018/06/vula-mbile.jpg)
# Project Scope

This repository contains the test automation code for user
interface based functional test automation. 

In this repo you will find:

- Tools used for setting up the testing environment in both iOS and Android.
- ADB (Android Debug Bridge) commands.
- Git branching strategies implemented on the project.
- pipenv virtualized environment.

 

# Environment 

|Tools                       |  Links to the download sites                                        |
| -------------------------- | ------------------------------------------------------------------  |
|android studio              |https://developer.android.com/studio/install                         | 
|appium for mac              |https://www.swtestacademy.com/how-to-install-appium-on-mac/          |
|appium for ubuntu           |http://testingalert.com/steps-to-setup-appium-on-ubuntu/             |     
|Python 3                    |https://realpython.com/installing-python/                            |          
|chromedriver                |http://chromedriver.chromium.org/downloads                           |  
|emulator (genymotion)       |https://www.genymotion.com/fun-zone/                                 |  
|pip3                        |https://www.shellhacks.com/python-install-pip-mac-ubuntu-centos/     |
|pipenv                      |https://packaging.python.org/tutorials/managing-dependencies/#managing-dependencies|

# ADB Usage


Android Debug Bridge (adb) is a versatile command-line tool that lets you communicate with a device. 
The adb command facilitates a variety of device actions, such as installing and debugging apps, and it provides access to a Unix shell that you can use to run a variety of commands on a device.
It is a client-server program that includes three components.

For more on adb : https://developer.android.com/studio/command-line/adb

Use the command below to kill the server

$ adb kill-server 

Use the command below to start server

$ adb start-server

Use the command below to list connected devices

$ adb devices 

Use the command below to connect to the specific device

$ adb connect < device name> 


To clone the repository follow the link below:

https://bitbucket.org/kineticskunk/vula_mobile_functional_test_automation/src/master/

# Branching strategies
//must have a seat down with the team and formulate branching strategy as accordance to 
the below git branches.

- Master 
- dev 
- enhancement / feature / register
- feature/ios_register
- feature/profile_picture
- feature/register
- ios_configuration
- login_feature

# Activate the pipenv shell

install pipenv following this command

cd into the project directory where it is cloned/downloaded then run the following command.

$ cd vula_mobile_functional_test_automation

Activate a pipenv shell inside the project directory with the following command.

$ pipenv shell
 
# Running the tests 

Make sure emulators and simulators have started on Mac Ubuntu OS.

Follow this link on how to start and choose a genymotion emulator device. 
https://docs.genymotion.com/latest/Content/01_Get_Started/Basic_steps.htm#basic-steps

Follow this link on how to start and choose a simulator device.
https://developer.apple.com/library/archive/documentation/IDEs/Conceptual/iOS_Simulator_Guide/GettingStartedwithiOSSimulator/GettingStartedwithiOSSimulator.html

Start the appium-server on ubuntu following the command below.

$ appium 

Start the appium-server on MAC OS by clicking on the appium icon.

# Running the tests (end to end)

$ behave android_behave

# Running the tests in Sequence (Individual Tests)


1.behave android_behave/ --tags=login

2.behave android_behave/ --tags=register

3.behave android_behave/ --tags=terms_conditions


# Tests 

|Name                        | Status     |Link to Trello Tickets |
| -------------------------- | ---------  | ------------  |    
|login                       |    Done    |  https://trello.com/b/jcJ4VM27/vula-mobile             |
| register                   |   Done     |               |    
|login and reset password    |   Not yet started|           |
|Check menu                  |   Not yet started|           |
|Check Patient list          | Not yet started  |           |
| Start referral             | Not yet started|             |   
| On call / off-duty indicator           | Not yet started |             
|Burns referral             | Not yet started |             |            
|Opthalmolgy referral form  | Not yet started |             |
|Other basic forms          | Not yet started |             |
|Backwards Compatibility    |Not yet started  |             |

# TODO 
-Insert a table for with trello links for feature tickets.
-Report generation articulation using junit.
-Implement branching strategy.
-Add more tests commands as we progress through the project.
