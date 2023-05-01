Download Link: https://assignmentchef.com/product/solved-bbm465-project-2-cyrpt-messenger
<br>
You are expected to develop a simple file client-server encryption/decryption messaging application.

The requirements are below:

<ul>

 <li>The program must support three encryption modes (CBC, OFB) and two encryption algorithms (AES, DES).</li>

 <li>Padding mode must always set to “PKCS5 Padding”  The program must be executed as follows:</li>

</ul>

Server: The server applications should be started first and wait for incoming connections. All encrypted messages received by the server will be distributed to clients directly. Besides, when the server starts, it will produce a random key and random initialization vector (IV) and send these key and vector to all the clients. Finally, the server must write, produced random key, produced IV and the encrypted message sent to itself with information about user name who sent the message to it’s console and must create/update a log file (log.txt) whenever a message is sent to itself (<strong>All these informations must be in Base64 Encoded (except “username”, username will be displayed as normal text</strong> )

Client: Client application should have similar GUI showed in Figure-1. In the GUI There are three textboxes. First and the biggest textbox is for messages. Incoming messages will be displayed in this textbox. Second textbox titled <strong>text</strong> is for message writing. After typing a message user will press encrypt button to cipher the message.  The encryption method and mode can be selected by using radio buttons top of the window.  Then user should press send button to send encrypted message to server.







Figure-1 GUI of the application.




<strong>Software usage. </strong>

First Client application has to connect to server via TCP/IP sockets. Then users should enter his/her nickname that will be used in chatting. The dialog box opened after pressing connect is displayed in Figure-2. The encrypted texts and decrypted texts should be displayed in message area as shown in Figure-3







Figure-2 Username dialog box.













Figure-3 Sample messages




All messages should be send to all clients. Encrypted and decrypted messages should be displayed on message textbox (<strong>crypted message must be</strong> <strong>displayed with Base64 encoded version</strong>).




The same encryption algorithm and mode should be selected in all clients. Key  and IV should be randomly generated by the server and distributed to all clients. All clients should use the same key and IV. You must use Java crypto API [1]  for encryption functions.

<strong> </strong>

<strong> </strong>

<h1>1               Notes</h1>

<ol>

 <li>You can ask questions about the experiment via Piazza group (piazza.com/hacettepe.edu.tr/fall2020/bbm465).</li>

 <li>Late submission will not be accepted!</li>

 <li>You must compile your program on Java version of the dev machine.</li>

 <li>You are going to submit your experiment to online submission system:</li>

</ol>

<a href="http://submit.cs.hacettepe.edu.tr/">http://submit.cs.hacettepe.edu.tr/</a>




The submission format is given below:

<em>&lt;</em>Group id<em>&gt;</em>.zip <em>−</em>[src]/

<em>−−</em>*.[java]





