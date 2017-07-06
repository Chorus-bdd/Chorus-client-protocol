# Chorus-client-protocol

From Chorus version 3.0.x (in Beta) clients can connect to Chorus and pubish their steps over a Web Socket connection

This  enables distributed Chorus tests to interact with any distributed components or microservices which can open a web sockets connection and send/receive messages over it. A primary target for this type of testing is Javascript/browser clients. However, our goal is to provide libraries to faciliate this for commonly-deployed languages.

This repo defines the messages which flow backwards and forwards over the web socket, to enable client components to connect and publish steps, and to enable the Chrous interpreter to request the execution of a test step and wait for the result to be sent. 

Although Web Sockets are the only transport presently, the message definitions should be considered a higher level protocol and an alternative message transport could be used in the future

Current client implementations for Chorus Web Socket client exist in Java (in the core Chorus project) and in Javascript (in the chorus-js repo)

