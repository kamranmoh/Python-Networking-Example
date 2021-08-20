# Python-Networking-Example
Ref YouTube channel: buildwithpython 

Title: Making a reverse shell connection

Direct connection: I am requested to help my friend. To connect to a friend’s computer, I need him to send his ip address and port to me. Using his and my ip /port I can build a socket which connects us. But this scenario has several limitations:
1-	Is he tech savvy to send ip and port to me?
2-	Ip is dynamic and changes after a restart
3-	Firewalls do not permit this type of connection
Reverse connection: In this scenario, which is similar to a hacker, the process starts from friend’s computer.  I make a python file which includes my ip and port and send it to my friend and when he opens the file it automatically creates a connection with me. As my friend is the initiator, I don’t need to worry about what is his ip address even if the ip address is dynamic, because every time the ip address changes it will be calibrated accordingly. This method is better than the direct method, but there is a problem with my ip address, which is also dynamic. It means when I make a file and send it to my friend the ip of my computer shall be included and therefore the file is only valid until I restart my computer. 

Two python files are prepared which shall run on the two computers ready for networking: RS_server and RS_client
I can send the client code to my friend as an exe file in case he does not have access to Jupyter or python. 

Procedure:
I run my RS-server which brings me to a waiting mode for my client. As soon as my friend runs the RS_client on his system, I will get a message that he is connected. Then I can use command line to apply changes.
