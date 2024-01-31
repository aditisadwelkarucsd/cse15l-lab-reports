# Lab 2 Report

Code behind ChatServer:
![Image](chatserver.png) 

**First time adding to the chat:**  
The method handleRequest in the Handler class is called once the url qeury has been made. In the method, it goes into the if block that handles the `/add-message` formatted query. The argument relevant for this method is the url, from which the function extracts the query and its parameters. There is only one relevant field in this class, the string `str` that contins the entire chat. When the `/add-message` request is made, the code extracts the user and the text from the query and appends it to the chat. The chat thus contains a record of every user and their corresponding text. In this screenshot, we append the message `Hello` said by the user `aditi`, to the chat, as follows:  

![Image](sc1.png)  

Second time adding to the chat:
![Image](sc2.png) 


Which methods in your code are called?
What are the relevant arguments to those methods, and the values of any relevant fields of the class?
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
By values, we mean specific Strings, ints, URIs, and so on. "abc" is a value, 456 is a value, new URI("http://...") is a value, and so on.)
