# STM32F746 Discovery - LVGL Demo Port

---

## Introduction

This project was designed to be used with the STM32F746G Discovery. 
One could normally find this project, as an STM32CubeIDE project, 
and that worked okay to build the original project, but I aim to 
expand with some custom demos, and I'd like to use PlatformIO 
as much as I can. It has been a fun exercise, cutting and pasting 
the requisite folders, but I was able to get it working with 
PlatformIO. 

---

## Demo Usage

To utilize the different demos, which I don't really recommend, but 
you'll want to check out the file in: lib > STM32F7 > lvgl > lv_conf.h 

In this file, you'll be able to find the following options:

    LV_USE_DEMO_WIDGETS
    LV_USE_DEMO_BENCHMARK
    LV_USE_DEMO_STRESS
    LV_USE_DEMO_MUSIC

Just set the value of this variable to 1, and the rest to 0. Then in the 
main.c file, you can comment the appropriate function call, and then the 
corresponding header. Often what I do is uncomment the function call, and
in CLion, I click on the suggested fixes, which suggests the proper import.

---

## Many Thanks

Many thanks to the lvgl team for their original port to this device. 
See the original port here:

https://github.com/lvgl/lv_port_stm32f746_disco

