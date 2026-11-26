# Lab 03 — Wireshark Protocol Analysis

## Objective
Learn to interpret DNS, TCP and TLS connection setup using self-generated traffic in an authorized lab.

## Capture workflow
1. Use a local lab VM or a system you own.
2. Start a capture on the correct interface.
3. Generate a small number of known DNS and HTTPS requests.
4. Stop the capture and save a sanitized copy.
5. Inspect protocol hierarchy, endpoints and conversation statistics.
6. Follow a TCP stream only where payload inspection is lawful and appropriate.
7. Record observations without including credentials, cookies or personal data.

## Useful display filters

```text
dns
tcp
tcp.flags.syn == 1
tls.handshake
icmp
```

## Questions to answer
- Which DNS query preceded the connection?
- Was the TCP three-way handshake completed?
- Was TLS negotiation successful?
- Are retransmissions, resets or timeouts visible?
- Does the timing suggest name-resolution, network or application delay?

## Evidence
Include screenshots only after checking that packet details, hostnames, IP addresses, payloads and identifiers are safe to publish. Prefer a regenerated synthetic capture.

## Authorization
Capture only traffic you own or are explicitly authorized to inspect. Do not intercept other users' traffic or bypass encryption.
