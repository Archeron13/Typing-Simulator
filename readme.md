# Keyboard-Simulator

## Requirements
To install the required library write the following command in your terminal after opening the directory where you have extracted the ZIP

```bash 
pip3 install -r requirements.txt
```

(Note you might need to get Tkinter by yourself as PIP does not offer it for some version of python.)

## Features

- Graphical User Interface
- Logging statistics such as CPM (Characters Per Minute), CPS (Character Per Second), Accuracy etc
- Saving the abovementioned statistics in a score.txt
- Choosing your own file from which the text will be displayed from.
- Restart button
- End button to get statistic mid-way instead of until the end of text
- Heatmap: to shows the letter the user gets wrong the most 


## Working

The main mechanism of this program,that is detecting keystroke is done by the use of the binding functionality of Tkinter to bind any event to the main windown and check whether the keypressed is the same as the one that is in the given text.
Tkinter is a bare-bone library and doesn't offer the functionality of dynamically resizing background image, luckily it is very easy to implement and 
I had problem with how to implement the restarting function since you cannot restart a thread once you stop it. I tried to create a thread manager but I didn't find success so I decided to just change the iterator in the thread's loop to restart the function.

## Running the simulator
```bash 
python main.py
```
