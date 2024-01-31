# Lab 2 Report
Show the code for your ChatServer, and two screenshots of using /add-message.

Code behind ChatServer:
`  public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return str; 
        } else {
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("&");
                String[] text = parameters[0].split("=");
                String[] user = parameters[1].split("=");
                if (text[0].equals("s") && user[0].equals("user")) {
                    str += (user[1] + ": " + text[1] + "\n");
                    return str; 
                }
            }
            return "404 Not Found!";
        }
    }`

For each of the two screenshots, describe:

Which methods in your code are called?
What are the relevant arguments to those methods, and the values of any relevant fields of the class?
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
By values, we mean specific Strings, ints, URIs, and so on. "abc" is a value, 456 is a value, new URI("http://...") is a value, and so on.)
