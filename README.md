# Socket-Programming-with-UDP

Java programming to help create and demonstrate an example of a UDP communication protocol. 

UDP allows two or more processes running on different hosts to communicate. UDP is a connectionless service - there is no handshaking to establish a communication pipe because UDP does not have a pipe. When UDP communicates, it attaches the destination address to each batch of data that is being sent  In UDP, the destination address is the IP address of the host and port number.  The host IP address, the port number and the actual data to be transferred are collectively called a ‘packet’. UDP provides an unreliable message-oriented service model, in that it makes a best effort to deliver the packet to the destination in a single operation at the sending side. UDP is a best-effort service; it makes no guarantee that the packet will be delivered. This is in contrast to TCP, which has a reliable service model.

1. The client reads a line from its standard keyboard and sends the line out from its socket to the server.
2. The server reads the line from the socket.
3. The server converts the line to upper case.
4. The server sends the modified line out of its socket to the client.
5. The client reads the modified line from its socket and prints it.

### The following diagram highlights the main activity of the UDP communication over a connectionless transport service.

<img width="881" alt="Screenshot 2021-09-13 at 19 34 26" src="https://user-images.githubusercontent.com/58150120/133138000-09cffede-299f-4e05-8e60-16cc67c26776.png">

### Local setup guide

A separate CMD prompt/terminal window is needed for the server and the client. 

Navigate to the folder where the Java files are (I would recommend putting them on the desktop) and compile the files using the following command "javac nameOfFile.java" - you will have to do that for both files. When compiled you are ready to run them. You will need to open a CMD/terminal window for the server and the client. When you have that set up you can run the server and client by typing "java nameOfFile" then Enter.

If you type a short message in the client window  - press Enter - it will be sent to the server. When it reaches the server it will be converted to UPPER CASE and sent back to the client with the message

Use Wireshark to capture the data and see what's going on with the process between the client and the server. You can download Wireshark for Windows and Mac. Set up your client and server as below and run Wireshark (select the loopback from the list of connections to monitor). Click the green fin and it will start monitoring the local loopback IP address 127.0.0.1. When you send your message from the client to the server Wireshark will capture it. Stop Wireshark (click red button). Scroll the captured data and look for 2 lines coloured light blue with the protocol UDP. One of them is the client to the server and the other is the server to the client. Click on them and you will see the information about the communication and you should see the message in the data window.

<img width="1003" alt="Screenshot 2021-09-13 at 19 42 37" src="https://user-images.githubusercontent.com/58150120/133139098-2e0c9fb4-a46b-47b1-87be-7e77f910631c.png">


