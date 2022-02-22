# STM32F429BITx HAL

This repository contains new project starter code for developing and building for STM32F429BITx using code generated for STM32F429BITx in STM32CUBEMx.
It uses Cmake and Ninja to generate .bin,  .elf, .hex and other files in the project build directory.

## Code generation

STM32CUBEMx is used to generate HAL code for STM32F429BITx. Pin and clock configurations  are done by the user.

**Requirement for this project setup is that you select STM32CUBEide toolchain for code generation**

The generated code will be inside your chosen folder. 

##  Project setup

* Clone this repository to your local machine
* Delete .git folder  ```rm -rf .git```
* Run  ```./install_dependencies.sh``` to install all the required dependencies.
* Copy the contents of the hall generated code into the ```stm32f429bi``` folder in the your project subdirectories.
* Move the two folders inside ```Core```, that is ```Inc``` and ```Src``` to the upper level directory. (replacing the two Inc and Src directories at the upper level)
* Open your vscode inside the ```your_project``` directory. Install any dependencies if asked.
* VScode cmake will pop up asking for the toolchain, selecte ```GNU.... custom toolchain``` 
* Configure  cmake in vscode by invoking ```ctrl+shift+p``` and selecting ```CMake::configure```
* Add your code to the top ```Src``` and ```Inc```  and inside the file ```main.c``` file.

## Video
coming soon