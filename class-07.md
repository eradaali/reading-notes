##
## Who is Roy Fielding?
 Some guy. He's smart, and  he do a servel of things 
  helped write the first web servers, that sent documents across the internet… and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.

  ## How does that work,The web?
  The protocol I mentioned, that he helped write, HTTP, it's capable of all sorts of neat stuff that people ignore for some reason,That first part tells the browser what protocol to use. That stuff you type in there is one of the most important breakthroughs in the history of computing ,Because it is capable of describing the location of something anywhere in the world from anywhere in the world. It's the foundation of the web. 

  **A web page is  a resource?**
   A web page is a “representation” of a resource. Resources are just concepts. URLs--those things that you type into the browser.

**what a URL is?**
URLs tell the browser that there's a concept, somewhere. A browser can then go ask for a specific representation of the concept. Specifically, the browser asks for the web page representation of the concept.

## HTTP—this protocol 
**The Hypertext Transfer Protocol (HTTP) is designed to enable communications between clients and servers.**

HTTP works as a request-response protocol between a client and server.
when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.

## Why can't a machine understand a normal web page?
 Because web pages are designed to be understood by people. A machine doesn't care about layout and styling. Machines basically just need the data. Ideally, every URL would have a human readable and a machine readable representation. When a machine GETs a resource, it will ask for the machine-readable one. When a browser GETs a resource for a human, it will ask for the human-readable "representation" of that data.

## HTTP Methods
   - GET :GET is used to request data from a specified resource.
   - POST :POST is used to send data to a server to create/update a resource.
   - PATCH :method supplies a set of instructions to modify the resource.
   - HEAD
   - DELETE :The DELETE method deletes the specified resource.
   - PUT :PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource
   - OPTIONS:The OPTIONS method describes the communication options for the target resource.
