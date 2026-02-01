# defence-pipeline-prototype
A project for prototyping a C++ based devOps stack

Requirements to run:
!!Incomplete!! - in works

On ubuntu install: 
- system temp sensors, 
- C++, 
- cmake
- libsensors-dev

sudo apt update
sudo apt install lm-sensors libsensors-dev build-essential cmake



seeing the lm-sensors in terminal yourself
json: sensors -j
updating (1s period) data on cmd: watch -n 1 -d sensors


libsensors has deprecated cmake version in use:
change first line of CMakeLists.txt to
- cmake_minimum_required(VERSION 3.10...3.25)


