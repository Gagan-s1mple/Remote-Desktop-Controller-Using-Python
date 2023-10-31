# Remote-Desktop-Controller-Using-Python
Remote Control App
This Python application allows you to control multiple computers remotely using a virtual touchpad and keyboard input.

Usage
Install Dependencies:

Before running the application, make sure to install the pyautogui module. You can do this by running the following command:
bash
Copy code
pip install pyautogui
Set Up Server and Clients:

Download server.py onto one computer and client.py onto the rest.
Run Server:

On the computer where you downloaded server.py, run the following command:
bash
Copy code
python server.py
Note the IP address and port displayed in the alert.
Run Clients:

On the other computers, run the following command for each client:
bash
Copy code
python client.py
When prompted for Host IP Address and Port, enter the details from the server's alert.
Using the Touchpad:

Click inside the tkinter window on the server computer to activate the virtual touchpad. The cursor will move simultaneously on the client computers.
Additional Controls:

Use Control + l for left click, Control + r for right click, and Control + d for double click. Dragging functionality is currently under development.
Typing Text:

Click on the 'Text' button in the touchpad menu. Enter your text in the provided field and click 'Type Text' to input on the clients. Use 'Delete' for backspace and 'Enter' for a new line.
