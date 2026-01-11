## Day 13 – DNS Debugging

First checks:
- /etc/resolv.conf
- getent hosts
- dig

Observations:
- Configured nameservers:
- Domain resolution result:
- Query time:

Key learnings:
- DNS is independent of routing
- IP success + domain failure = DNS
- /etc/hosts overrides everything

Production mindset:
- Always test DNS explicitly
- Never assume DNS is “fine”
