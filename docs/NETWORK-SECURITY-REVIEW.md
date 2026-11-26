# Network Security Review Checklist

## Architecture and segmentation
- [ ] Trust zones and asset owners documented
- [ ] User, server, management, security and OT networks separated as required
- [ ] Inter-zone flows justified and approved
- [ ] Default-deny policy applied where appropriate
- [ ] Shared services and third-party connectivity reviewed

## Secure administration
- [ ] Management interfaces not exposed directly to the internet
- [ ] Administrative access uses approved jump/Bastion or privileged access path
- [ ] MFA and role separation enforced
- [ ] Device management plane restricted and logged

## Network services
- [ ] DNS, NTP, PKI and IPAM dependencies understood
- [ ] Routing and failover behavior documented
- [ ] Load balancer health checks and TLS settings reviewed
- [ ] Remote access and VPN posture assessed

## Monitoring and lifecycle
- [ ] Firewall decisions and critical flows logged
- [ ] Alerts have owners and response procedures
- [ ] Rules include purpose, owner, change reference and review date
- [ ] Temporary exceptions expire or are recertified
- [ ] Config backups and recovery are tested

## Evidence
Record scope, reviewer, date, findings, severity, owner and target closure date. Keep production configuration and topology in controlled systems, not this public portfolio.
