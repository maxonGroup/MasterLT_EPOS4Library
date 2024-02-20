# MasterLT_EPOS4Library
The EPOS4 Class Library can be used to control the maxon EPOS4 digital positioning controllers using the maxon motor Australia MiniMaster LT/MicroMaster LT CANopen Master Controllers. 
This repository contains the library and header file for the EPOS4 Class Library that can be imported into your custom C++ projects. 

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li> <a href="#getting-started">Getting Started</a> </li>
    <li><a href="#useful-documents">Useful Documents</a></li>
    <li><a href="#feedback">Feedback</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>


<!-- GETTING STARTED -->
## Getting Started

The instructions provided here are aimed to setup Visual Studio Code (VS Code) as the IDE. 

* Install [VS Code](https://code.visualstudio.com/)
* Add the platformio extension
* Add C/C++ instellisense extension (if not done automatically)
* Download [Git](https://git-scm.com/downloads)

Please refer to the README file in the [MasterLT_EPOS4Demo repository](https://github.com/maxonGroup/MasterLT_EPOS4Demo) on details on how to set up the example project. 

The following instructions assume you have set up a platformio project containing a ```.ini``` file. 

The  ```.ini``` file contains the following code:

```
; PlatformIO Project Configuration File
;
;   Build options: build flags, source filter
;   Upload options: custom upload port, speed and extra flags
;   Library options: dependencies, extra library storages
;   Advanced options: extra scripting
;
; Please visit documentation for the other options and examples
; https://docs.platformio.org/page/projectconf.html
[env:development]
platform = espressif32@6.5.0
board = esp32doit-devkit-v1
framework = espidf
monitor_speed = 115200
debug_tool = esp-prog
monitor_filters = esp32_exception_decoder
lib_deps = https://github.com/maxonGroup/MasterLT_EPOS4Library.git#v0.10.0
```

A key point of interest is the ```lib_deps``` field. 
This field is how you import the contents of this library to your project. 
The tagged release version is specified in the field after the  ```#```.
The version numbers follow the semantic versioning convention.
Rebuild the platformio project after the .ini file has been modified. 


## Useful Documents

* [EPOS4 Class Library Documentation](https://www.maxongroup.net.au/medias/sys_master/root/9233349345310/2402-EPOS4Class-Documentation.pdf) 
* [MasterLT_EPOS4Demo repository](https://github.com/maxonGroup/MasterLT_EPOS4Demo)


<!-- Feedback -->
## Feedback

See the [open issues](https://github.com/maxonGroup/MasterLT_EPOS4Demo/issues).

Please post issues and comments here. 


<!-- CONTACT -->
## Contact

For any queries, please contact:
* Dr. Carlos Bacigalupo - carlos.bacigalupo@maxongroup.com
* Mr. Mihir Joshi - mihir.joshi@maxongroup.com

Project Link: [https://github.com/maxonGroup/MasterLT_EPOS4Library](https://github.com/maxonGroup/MasterLT_EPOS4Library.git)

