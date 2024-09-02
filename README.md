# PRODIGY_CS_04
This is a basic keylogger script written in Python using the pynput library. The script captures keystrokes and logs them into a text file.

Features
Keystroke Logging: Captures all keystrokes, including special keys (e.g., Shift, Enter, Backspace), and writes them to a log file.
Log File: The captured keystrokes are saved in a specified text file on your system.
Requirements
Python 3.x
pynput library
You can install the pynput library using pip:

bash
Copy code
pip install pynput
How to Use
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/simple-keylogger.git
cd simple-keylogger
Edit the file path:

Update the file path in the script to the desired location where you want to save the keystroke log:

python
Copy code
log_file_path = r"C:\Users\kanis\OneDrive\Desktop\Simplekeylogger.txt"
Run the script:

bash
Copy code
python simple_keylogger.py
The script will start logging keystrokes and save them to the specified log file.

Stop the keylogger:

To stop the keylogger, you can close the terminal or use an interrupt (Ctrl + C).

Code Overview
keyPressed(key): Callback function that handles the event when a key is pressed. It logs the keystroke to a file.
keyboard.Listener: Listens for keyboard events and calls the keyPressed function when a key is pressed.
Log File: Keystrokes are appended to a text file, with special keys indicated in brackets (e.g., [Key.enter]).
