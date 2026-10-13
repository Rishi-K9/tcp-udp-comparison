# TCP and UDP Comparison

## Project Overview

This project compares Transmission Control Protocol (TCP) and User Datagram Protocol (UDP), two transport-layer protocols used for communication over IP networks.

## Objective

To understand the differences between TCP and UDP in terms of reliability, connection behaviour, protocol overhead, and suitable use cases.

## Tools Used

- Web Browser
- GitHub
- Wireshark

## Approach

1. Reviewed the basic functions of TCP and UDP.
2. Compared connection behaviour, reliability, acknowledgments, retransmission, and protocol overhead.
3. Identified common applications and use cases for both protocols.
4. Documented the comparison and findings in `report.md`.

## TCP vs UDP Comparison

| Feature | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented | Connectionless |
| Reliability | Reliable delivery | No built-in delivery guarantee |
| Data Ordering | Preserves byte-stream order | No built-in ordering guarantee |
| Acknowledgments | Supported | Not built in |
| Retransmission | Supported | Not built in |
| Overhead | Generally higher | Generally lower |
| Flow Control | Supported | Not provided by UDP itself |
| Congestion Control | Supported | Not provided by UDP itself |
| Common Use Cases | Web traffic, email, file transfers | Real-time media, online gaming, DNS |

## Key Learnings

- TCP provides reliable and ordered delivery of a byte stream.
- UDP sends independent datagrams without establishing a transport-layer connection.
- TCP includes flow control and congestion control.
- UDP has lower protocol overhead and is often useful for latency-sensitive applications.
- Protocol selection depends on the application's reliability and latency requirements.

## Project Structure

- `README.md` - Project overview and key findings.
- `report.md` - Detailed TCP and UDP comparison report.

## Testing and Evidence

The report documents protocol characteristics and common use cases. Packet captures and empirical performance measurements have not yet been documented.

## Deployment Configuration and Rollback Evidence

This project is a networking protocol comparison report rather than a deployable software application. No application deployment or rollback has been performed.

## Conclusion

TCP is appropriate when reliable and ordered delivery is essential. UDP is often appropriate for latency-sensitive applications that can tolerate packet loss or implement recovery mechanisms separately.

## References

- [Wireshark Official Website](https://www.wireshark.org/)
- [RFC 9293: Transmission Control Protocol (TCP)](https://www.rfc-editor.org/rfc/rfc9293)
- [RFC 768: User Datagram Protocol (UDP)](https://www.rfc-editor.org/rfc/rfc768)

## Change Verification

This section was added to verify the Git-based change and rollback workflow for this documentation repository.
