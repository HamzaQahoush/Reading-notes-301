### Client/server architecture :
when a client (usually a web browser) 
sends a request to a server (most of the time a web server ), using the HTTP protocol. 
The server answers the request using the same protocol.

![](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)


The `<form>` element defines how the data will be sent. All of its attributes are designed
to let us configure the request to be sent when a user hits a submit button. The two most important attributes are `action` and `method.`

The `action` attribute defines where the data gets sent. Its value must be a `valid relative` or `absolute URL`.

The method attribute
The method attribute defines how data is sent.

The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted 
via a number of different methods, the most common being the GET method and the POST method

### HTTP Methods
• The GET method
The GET method is the method used by the browser to ask the server to send back a given resource.

• The POST method
It's the method the browser uses to talk to the server when asking 
for a response that takes into account the data provided in the body of the HTTP request.

### Viewing HTTP requests :

1.Open the developer tools.\
2.Select "Network"\
3.Select "All"\
4.Select "foo.com" in the "Name" tab\
5. "Headers"

![](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/network-monitor.png)
