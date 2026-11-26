# Lab 02 — DNS Troubleshooting

## Objective
Practice structured DNS troubleshooting using a domain and records you own or a safe public test domain.

## Workflow
1. Confirm the client resolver configuration.
2. Query the configured resolver and compare with an approved alternate resolver.
3. Check A/AAAA, CNAME, MX and TXT records as relevant.
4. Inspect TTL and authoritative response.
5. Compare expected and observed results.
6. Check whether the issue is client cache, recursive resolver, authoritative DNS or application configuration.

## Example commands

```bash
nslookup example.com
dig example.com A
dig example.com MX
dig +trace example.com
```

## Interpretation checklist
- Is the queried name correct?
- Does the response code indicate success, no data or failure?
- Is the answer authoritative or cached?
- Does TTL explain a propagation delay?
- Are split-horizon or conditional-forwarding rules involved?
- Is the application using the resolver you tested?

## Safety
Do not enumerate private zones or publish internal DNS names, resolver addresses, zone transfers or customer records. Use domains you control or public test domains.
