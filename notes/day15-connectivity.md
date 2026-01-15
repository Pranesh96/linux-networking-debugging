## Day 15 – Network Connectivity Investigation

Incident summary:
- Symptom: Website not reachable externally
- Scope: External users only

Investigation steps:
1. Interface & IP – verified interface UP with valid IP
2. Routing – default gateway present and reachable
3. DNS – domain resolved correctly
4. Service – service running and listening
5. Port reachability – local OK, remote failing
6. Firewall – suspected blocking traffic

Findings:
- Local connectivity successful
- External connection timed out
- Indicates firewall or upstream block

Root cause (hypothesis):
- Inbound firewall rule blocking port 80

Corrective action:
- Review and update firewall rules

Preventive measures:
- Add monitoring for port reachability
- Document firewall changes

Key lesson:
- Always test locally vs remotely to isolate cause
