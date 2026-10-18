# Networking Fundamentals: Connectivity Checks

## Objective

Learn how to inspect network configuration, understand DNS resolution, and perform basic connectivity checks.

## Lab Environment

- Windows 11
- Ubuntu on WSL, when applicable
- Standard networking utilities

## Exercise 1: Inspect Network Configuration

### Windows

```powershell
ipconfig
```

Observe the IPv4 address, subnet mask, and default gateway for the relevant network adapter.

### Ubuntu / Linux

```bash
ip addr
ip route
```

Observe the network interfaces and routing information.

## Exercise 2: Check DNS Resolution

```bash
nslookup example.com
```

Observe whether the hostname resolves to an IP address. Record the result and explain what DNS does.

## Exercise 3: Test Connectivity

### Windows

```powershell
ping -n 4 example.com
```

### Ubuntu / Linux

```bash
ping -c 4 example.com
```

Record whether replies were received, any packet loss, and the reported round-trip times.

Note: A failed ping does not always mean the destination is offline. ICMP traffic may be blocked.

## Exercise 4: Troubleshooting Observations

For each command, document:

1. What the command checks
2. The actual result
3. What the result indicates
4. One possible reason for a failure

## Key Concepts

- IP address: identifies a network interface within an IP network.
- Default gateway: provides a route to networks beyond the local network.
- DNS: translates domain names into DNS records, commonly IP addresses.
- Ping: tests reachability using ICMP echo messages when permitted.

## Safety

These exercises use standard diagnostic commands and a public example domain. Only investigate systems and networks you are authorised to test.

## Results

Add your own observations after running each command. Do not invent outputs or publish sensitive network details.
