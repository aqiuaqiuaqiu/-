一个自动化工具，有图片识别、键鼠操作。
做这个的初衷是游戏中摆摊时有时因为网络问题会掉线，这个时候需要加速器切换一个线路。
但是我们又没在电脑前，所以这个自动化执行工具可以设定指定时间内切换线路，以防止掉线。
后来索性增加了一些自动化命令，通过excle就可控制，可以让更多人使用，使用场景也不局限于切换加速器线路。
基本可以满足绝大部分自动化场景。


配置文件夹如图，如果自动化过程中有需要识别的图片放在这个文件夹。
![image](https://github.com/aqiuaqiuaqiu/lianxi3/assets/168556559/b3878310-41eb-42d3-9fa9-a38773f6704a)

peizhi.xlsx是命令文件，内容是这样：
![image](https://github.com/aqiuaqiuaqiu/lianxi3/assets/168556559/7c4bf902-bc32-41a9-80be-f272607bb72e)

有命令说明：
![image](https://github.com/aqiuaqiuaqiu/lianxi3/assets/168556559/a8ecb47a-c9ab-4c3e-bf5c-a4013140cff4)


所依赖的库有如下：
import logging

import win32gui, win32con, win32com.client

import pygetwindow as gw

import time

import win32com.client as win32

import numpy as np

import cv2

import os

from mss import mss

import pyautogui

import pyperclip

import keyboard

from datetime import datetime

