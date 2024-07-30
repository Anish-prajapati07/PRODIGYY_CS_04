# PRODIGYY_CS_04
This is my **fourth task** of **Prodigy summer internship** in which I create a basic keylogger progam that records and logs keydtrokes.

In this, use various functions and library.

This **imports** the keyboard module from the **pynput** library, which is used for monitoring and controlling keyboard events.

**keyPressed(key)** is a function that is called whenever a key is pressed.

**print(str(key))** prints the representation of the key to the console. This is useful for debugging or seeing what keys are being pressed.

**with open("anish.txt", 'a') as logKey** opens the file "anish.txt" in append mode ('a'). If the file doesn't exist, it will be created. The with statement ensures that the file is properly closed after the block of code is executed.

Inside the **try** block, **key.char** attempts to get the character associated with the key press.

**logKey.write(char)** writes the character to the file.

if __name__ == "__main__": ensures that this block of code runs only if the script is executed directly, and not if it's imported as a module in another script.

**listener = keyboard.Listener(on_press=keyPressed)** creates an instance of keyboard.Listener, which listens for keyboard events. It is configured to call keyPressed whenever a key is pressed.

**listener.start()** starts the listener in a separate thread. This allows the main program to continue running while the listener waits for key events.

**input()** keeps the program running and waits for user input. This is necessary because otherwise, the script would terminate immediately after starting the listener, as there’s no other code to keep it alive.

**In short** ,

This script listens for key presses and logs them to a file named "anish.txt".

It uses pynput to capture keyboard events.

Characters from key presses are written to the file, while special keys are not logged.

The program remains active and waits for user input to prevent it from exiting immediately.





