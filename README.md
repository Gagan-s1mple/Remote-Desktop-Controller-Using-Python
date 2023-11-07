PROCEDURE:  
  
•	We first need to install the pyautogui module to control the cursor and keyboard. 
 
•	We now need to download server.py onto one of the computers and client.py to the rest. 
 
•	Now run server.py on and note the IP address as well as the port that comes as an alert. 
 
•	On the other computers, run client.py. When it asks for the Host IP Address and the Port, type the details that you saw in the alert. 
 
•	On the computer running server.py, you should now see a tkinter window. This window is your virtual touchpad. Click inside the window, and as your cursor moves inside that window, the cursor will move simultaneously on the client computers! 
 
•	You can adjust the window so that the touchpad can reach each end of the client computer. You can use Control + l for left click, Control + r for right click and Control + d for the double click. I am working on adding dragging functionality to the touchpad too! 
 
•	To type text, click on the 'Text' button from the menu of the touchpad. This should bring up a window. Use the text field to enter your text, and click on the 'Type Text' button to type the text on the clients, 'Delete' for 'backspace' and 'Enter' for a new line. 

 
 *Import Socket Library  
	To use a socket object in your program, start off by importing the socket library. No need to install it with a package manager, it comes out of the box with Python.  
