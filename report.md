TCP vs UDP Comparison Report
1. Objective

The objective of this task is to understand the differences between Transmission Control Protocol (TCP) and User Datagram Protocol (UDP), with a focus on reliability, connection behavior, overhead, and practical use cases.

2. Introduction

TCP and UDP are transport layer protocols used for communication between devices over IP networks. They differ in how they deliver data, handle errors, and manage communication between applications.

3. TCP vs UDP Comparison
Feature	TCP	UDP
Full Form	Transmission Control Protocol	User Datagram Protocol
Connection	Connection-oriented	Connectionless
Reliability	Provides reliable, ordered delivery	Does not guarantee delivery or ordering
Acknowledgments	Uses acknowledgments	No built-in delivery acknowledgments
Retransmission	Retransmits lost data when necessary	No built-in retransmission
Data Delivery	Provides a reliable byte stream	Sends independent datagrams
Overhead	Generally higher	Generally lower
Speed and Latency	May introduce additional delay due to reliability mechanisms	Often has lower protocol overhead
Flow Control	Supported	Not provided by UDP itself
Congestion Control	Supported by TCP	Not provided by UDP itself
Common Uses	Web traffic, email, file transfers	Real-time media, online gaming, DNS queries
4. How TCP Works

TCP establishes a connection using a three-way handshake:

SYN: The client requests a connection.
SYN-ACK: The server acknowledges the request.
ACK: The client acknowledges the server's response.

After establishing the connection, TCP uses sequence numbers, acknowledgments, retransmissions, and other mechanisms to provide reliable, ordered delivery of a byte stream.

5. How UDP Works

UDP sends independent datagrams without establishing a transport-layer connection first. It does not guarantee delivery, ordering, or duplicate protection.

Because UDP has a smaller protocol header and fewer built-in reliability mechanisms, it can be suitable for applications that prioritize low latency or implement their own reliability mechanisms.

6. Use Cases
TCP
Web browsing using HTTP/1.1 or HTTP/2 over TCP.
Email communication.
File transfers that require reliable delivery.
Applications that need ordered data delivery.
UDP
Real-time voice and video communication.
Multiplayer online games.
DNS queries in common configurations.
Applications that can tolerate some packet loss or implement their own recovery mechanisms.

Note: HTTP/3 uses QUIC over UDP, with reliability and congestion-control mechanisms implemented by QUIC.

7. Advantages and Limitations
TCP Advantages
Reliable and ordered data delivery.
Retransmission of lost data.
Built-in flow and congestion control.
TCP Limitations
Connection establishment adds overhead.
Retransmissions and ordered delivery can increase latency.
UDP Advantages
Small header and low protocol overhead.
No transport-layer connection establishment.
Useful for latency-sensitive applications.
UDP Limitations
No built-in guarantee of delivery or ordering.
Applications may need to implement reliability, congestion control, or recovery where required.
8. Conclusion

TCP is generally appropriate when reliable and ordered delivery is important. UDP is often appropriate when low latency and application-specific control are priorities. The best choice depends on the application's requirements rather than speed alone.

9. Interview Questions

Q1. What is TCP?

TCP is a connection-oriented transport-layer protocol that provides reliable and ordered delivery of a byte stream.

Q2. What is UDP?

UDP is a connectionless transport-layer protocol that sends datagrams without guaranteeing delivery or ordering.

Q3. When is UDP preferred?

UDP is often preferred for real-time communication, online gaming, and other latency-sensitive applications where occasional packet loss is acceptable or recovery is handled by the application or a higher-level protocol.
