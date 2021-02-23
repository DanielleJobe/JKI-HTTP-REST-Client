This document was created by the [PetranWay Autodocumentation Utility](https://bitbucket.org/ChrisCilino/labview-auto-documentation/src/master/).





# Charter

Empty



# Location

C:\Projects\JKI HTTP _ Doc\source\classes\REST Client\REST Client.lvclass



# Private Data

See the [Class Report Design](https://bitbucket.org/ChrisCilino/labview-auto-documentation/wiki/User%20Documentation/Confluence%20Report%20Printouts/Class) for an explanation of [data name](https://bitbucket.org/ChrisCilino/labview-auto-documentation/wiki/User%20Documentation/Confluence%20Report%20Printouts/Class#markdown-header-private-data-name) and [type](https://bitbucket.org/ChrisCilino/labview-auto-documentation/wiki/User%20Documentation/Confluence%20Report%20Printouts/Class#markdown-header-private-data-type) syntax.

|Name|Description|Data Type|
|-|-|-|
|Username||String|
|Password||String|
|cookie file||Path|
|verify server||Boolean|
|handle queue*||TypedRefNum|
|handle queue*.{}||Cluster|
|handle queue*.{}.client handle out*||TypeDef "ClientHandle": TypedRefNum|
|handle queue*.{}.client handle out*.Numeric||U32|
|handle queue*.{}.custom headers[]||1 Dimensional Array|
|handle queue*.{}.custom headers[].Header{}||TypeDef "HTTP Header": Cluster|
|handle queue*.{}.custom headers[].Header{}.header|**header** specifies the header field to add to all Web requests associated with the **Client Handle**. The **header** control provides a pull-down menu with some available header fields.|ComboBox|
|handle queue*.{}.custom headers[].Header{}.value|**value** specifies the value to assign to the header field. The default value is an empty string, which erases any value already associated with the specified **header**.|String|
|timeout (10000)||I32|
|headers[]||1 Dimensional Array|
|headers[].Header{}||Cluster|
|headers[].Header{}.header|**header** specifies the header field to add to all Web requests associated with the **Client Handle**. The **header** control provides a pull-down menu with some available header fields.|ComboBox|
|headers[].Header{}.value|**value** specifies the value to assign to the header field. The default value is an empty string, which erases any value already associated with the specified **header**.|String|
|Base URL||String|
|HTTP Header Bug||Boolean|
|Escape URLs||Boolean|




# Members

|Member Name|Scope|Dynamic Dispatch|Must Override|Must Use Parent Implementation|Description \ Prototype|
|-|-|-|-|-|-|
|Resolve Headers|private|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client/blob/master/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Create%20REST%20Clientc.png?raw=true" alt="Resolve Headersc.png" width="298" hieght="56" />|
|| | | | ||
|| | | | ||
|New Client Handle|private|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client/blob/master/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/New%20Client%20Handlec.png?raw=true" alt="New Client Handlec.png" width="328" hieght="132" />|
|| | | | ||
|| | | | ||
|Get client handle|private|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client/blob/master/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Get%20client%20handlec.png?raw=true" alt="Get client handlec.png" width="298" hieght="75" />|
|| | | | ||
|| | | | ||
|Return client handle|private|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client/blob/master/Developer-Resources/APIs/Images/REST-Client-Class-Documentation//Return%20client%20handlec.png?raw=true" alt="Return client handlec.png" width="298" hieght="75" />|
|| | | | ||
|| | | | ||
|Parse Status Line|private|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client/blob/master/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Parse%20Status%20Linec.png?raw=true" alt="Parse Status Linec.png" width="346" hieght="94" />|
|| | | | ||
|| | | | ||
|Resolve URL|private|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client/blob/master/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Resolve%20URLc.png?raw=true" alt="Resolve URLc.png" width="298" hieght="56" />|
|| | | | ||
|| | | | ||
|Error Handler|protected|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Error%20Handlerc.png" alt="Error Handlerc.png" width="298" hieght="75" />|
|| | | | ||
|| | | | ||
|Flush Client Handles|protected|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Flush%20Client%20Handlesc.png" alt="Flush Client Handlesc.png" width="298" hieght="42" />|
|| | | | |Destroy REST client reference.|
|| | | | ||
|HTTP Request|protected|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20Requestc.png" alt="HTTP Requestc.png" width="409" hieght="132" />|
|| | | | ||
|| | | | ||
|HTTP Header|public|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20Headerc.png" alt="HTTP Headerc.png" width="32" hieght="32" />|
|| | | | ||
|| | | | ||
|HTTP Methods|public|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20Methodsc.png" alt="HTTP Methodsc.png" width="32" hieght="32" />|
|| | | | ||
|| | | | ||
|Escape URL String|public|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Escape%20URL%20Stringc.png" alt="Escape URL Stringc.png" width="388" hieght="32" />|
|| | | | |Escape URL string.|
|| | | | ||
|Create REST Client|public|FALSE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Create%20REST%20Clientc.png" alt="Create REST Clientc.png" width="342" hieght="132" />|
|| | | | |The VI provides multiple arguments for defining how to create the JKI REST Client instance.  **Base URL** specifies the base URL to be used for the HTTP requests.  **Escape URLs** when true instruct the REST Client to escape all URLs before executing the requests. If you have already escaped the URLs, set this to false.  **Authentication** allows setting the username and password for services that use HTTP authentication.  **Verify Server** when true instructs the REST Client to validate the certificate of the server when HTTPS protocol is being used.  **Default Headers** specifies an array of headers to be used with every requests. Defaults to application/json content type.  **Cookie File** specifies a file path to be used for cookies.|
|| | | | ||
|HTTP HEAD|public|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20HEADc.png" alt="HTTP HEADc.png" width="364" hieght="113" />|
|| | | | |Perform a HTTP HEAD request.  The VI provides multiple arguments for defining how to perform the HTTP request.  **Path** specifies the path beneath the Base URL to be used for the HTTP request. request specific headers specifies an array of headers to be used with this particular HTTP request.   **request specific headers**The Default Headers specified upon creation of the JKI REST Client together with the request specific headers will all be used for the HTTP request.|
|| | | | ||
|HTTP GET|public|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20GETc.png" alt="HTTP GETc.png" width="364" hieght="113" />|
|| | | | |Perform a HTTP GET request.  The VI provides multiple arguments for defining how to perform the HTTP request.  **Path** specifies the path beneath the Base URL to be used for the HTTP request. request specific headers specifies an array of headers to be used with this particular HTTP request.   **request specific headers** The Default Headers specified upon creation of the JKI REST Client together with the request specific headers will all be used for the HTTP request.|
|| | | | ||
|HTTP PUT|public|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20PUTc.png" alt="HTTP PUTc.png" width="364" hieght="113" />|
|| | | | |Perform a HTTP PUT request  The VI provides multiple arguments for defining how to perform the HTTP request.  **Path** specifies the path beneath the Base URL to be used for the HTTP request.  **Request body** specifies the body of the request to be send to the server.  **request specific headers** specifies an array of headers to be used with this particular HTTP request. The Default Headers specified upon creation of the JKI REST Client together with the request specific headers will all be used for the HTTP request.|
|| | | | ||
|HTTP POST|public|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20POSTc.png" alt="HTTP POSTc.png" width="364" hieght="113" />|
|| | | | |Perform a HTTP POST request.  The VI provides multiple arguments for defining how to perform the HTTP request.  **Path** specifies the path beneath the Base URL to be used for the HTTP request.  **Request body** specifies the body of the request to be send to the server.  **request specific headers**  specifies an array of headers to be used with this particular HTTP request. The Default Headers specified upon creation of the JKI REST Client together with the request specific headers will all be used for the HTTP request.|
|| | | | ||
|HTTP POST Multipart|public|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20POST%20Multipartc.png" alt="HTTP POST Multipartc.png" width="364" hieght="113" />|
|| | | | |Perform a HTTP POST request and submits multiple sets of data or files.  The VI provides multiple arguments for defining how to perform the HTTP request.  **Path** specifies the path beneath the Base URL to be used for the HTTP request.  **Multipart Post data** data is the array of clusters specifying the data attributes and values to submit to the server (see the built-in LabVIEW HTTP Client's POSTMultipart VI documentation for details).  **request specific headers**  specifies an array of headers to be used with this particular HTTP request. The Default Headers specified upon creation of the JKI REST Client together with the request specific headers will all be used for the HTTP request.|
|| | | | ||
|HTTP DELETE|public|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/HTTP%20DELETEc.png" alt="HTTP DELETEc.png" width="364" hieght="113" />|
|| | | | |Perform a HTTP DELETE request.  The VI provides multiple arguments for defining how to perform the HTTP request.  **Path** specifies the path beneath the Base URL to be used for the HTTP request.  **request specific headers** specifies an array of headers to be used with this particular HTTP request. The Default Headers specified upon creation of the JKI REST Client together with the request specific headers will all be used for the HTTP request.|
|| | | | ||
|Destroy REST Client|public|TRUE|FALSE|FALSE|<img src="https://github.com/DanielleJobe/JKI-HTTP-REST-Client.git/wiki/Developer-Resources/APIs/Images/REST-Client-Class-Documentation/Destroy%20REST%20Clientc.png" alt="Destroy REST Clientc.png" width="262" hieght="42" />|
|| | | | |Destroy REST client reference.|
|| | | | ||
