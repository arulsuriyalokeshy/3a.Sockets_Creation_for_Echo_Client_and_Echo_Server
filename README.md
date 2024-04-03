# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
client:
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())

```

Server:
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())

```
## OUPUT
client:


![image](https://github.com/arulsuriyalokeshy/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/149130151/83d22389-f112-4640-8ac0-8be08cff987e)


Server:


![image](https://github.com/arulsuriyalokeshy/3a.Sockets_Creation_for_Echo_Client_and_Echo_Server/assets/149130151/a2d3438e-008d-4e58-99b5-d44f75eb62c3)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
