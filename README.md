# udp-tcp-chatRoom
Practice on udp and tcp to create a chat room with one server and multiple clients.   
  
For both UDP and TCP:  
Achieve a chat-room for multi-clients to communicate. User can either enter "all" to send messages within the registered group or use specific ip:port form to send personal message to another client.   
  
## For TCP:  
    Server.java is the main server file, which can fork the socket to the serverThread.java once it received a connection request.    
    ServerThread.java receives the message from sender and transfer it to the receiver.  
    ClientThread.java is the thread of a client, asking for the user inputs and send them. It also create a readThread.   
    ReadThread.java called by clientThread listens the reply from the server.  
  
## For UDP:   
    ChatRoomServer.java is the server and chatClient.java is the client thread. (chatClient.java create a thread in the main, and I created another client through running clientB.java. Same for TCP)  
    
 
