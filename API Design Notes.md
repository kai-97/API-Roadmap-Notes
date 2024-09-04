# API Design Notes

**Reference -** roadmap.sh/api-design

### Q. What are APIs?
- Way of communicating between software to share/transfer only essential information.
- GET, POST, PUT, DELETE
- Way of data exchange

## HTTP
### Q. What is HTTP?
- HyperText Trasnfer Protocol
- Used to transmit hypermedia data on the web. Hypermedia: JSON, HTML Webpages, JSON.
- Protocol that defines how content is requested and transmitted across the internet.

### Three Way Handshake
All TCP connections begin with a three-way handshake in which the client and the server share a series of packets before starting to share the applications data.

SYN - Sends 'x' to the server  
SYN ACK - Server acknowledges the request by sending ACK packet back to client. Sends back Y and X+1 for example  
ACK - Sends 'y+1' to the server  

Once the above (3 way handshake is complete, data transfer starts)

![image](https://github.com/user-attachments/assets/fb5fcfda-ab2b-4bfa-977a-2c16b5b0150e)

**Stateless Server**:
- Does not maintain the information about the client.  
- Each of the requests has to have the information necessary for the server to fulfil the request  
- Any request does not depend on any old request
- Thus, increased bandwidth usage as need to pass redundant data for connection
- And also make the same connections multiple times.
