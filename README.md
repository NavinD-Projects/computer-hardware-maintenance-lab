# Project 3: Basic Computer Networking and Troubleshooting

## Objective

Understand basic LAN concepts and use built-in Windows commands to inspect network configuration and troubleshoot simple connectivity problems.

## Concepts

- LAN: a network connecting devices in a limited area.
- IP address: a logical address used to identify a device on an IP network.
- Default gateway: the next-hop device used to reach other networks.
- DNS: translates domain names into IP addresses.
- DHCP: automatically provides network configuration to clients.
- Router: forwards traffic between networks.
- Switch: connects devices within a local network.

## Activities

Open Command Prompt. Run the commands below and record the output relevant to your own device.

### Activity A — Inspect IP configuration

```bat
ipconfig
ipconfig /all
```

Record the active adapter, IPv4 address, subnet mask, default gateway, and DNS servers. Do not publish public IP addresses or other sensitive network details.

### Activity B — Test connectivity

```bat
ping 127.0.0.1
ping <your-default-gateway>
ping 8.8.8.8
ping google.com
```

Replace `<your-default-gateway>` with the gateway shown by `ipconfig`. A failed ping does not always mean the network is down; some networks block ICMP.

### Activity C — Trace a route

```bat
tracert google.com
```

Observe the hops. Some routers may not respond, so timeouts are not necessarily a fault.

### Activity D — Basic troubleshooting sequence

1. Check Wi-Fi is enabled or the Ethernet cable is connected.
2. Confirm the device has an IP address.
3. Check the default gateway.
4. Test local connectivity.
5. Test external IP connectivity.
6. Test DNS by pinging a domain name.
7. Record results and escalate if the issue remains.

Do not change router settings or reset shared network equipment without permission.

## Simple network diagram

```text
Internet
   |
Router / Wi-Fi Access Point
   |
   +------ Laptop / PC
   |
   +------ Printer
```

Adapt this diagram to the network you actually tested.

## Evidence to add

Add your own redacted screenshots to `evidence/`:
- `ipconfig-redacted.png`
- `ping-tests-redacted.png`
- `tracert-redacted.png`
- `network-diagram.png`

Hide public IP addresses, Wi-Fi names if private, MAC addresses, internal hostnames, and other sensitive details.

## Completion checklist

- [ ] Explained LAN, IP, gateway, DNS, DHCP, router and switch.
- [ ] Ran `ipconfig` and `ipconfig /all`.
- [ ] Ran permitted ping tests.
- [ ] Ran `tracert`.
- [ ] Documented one troubleshooting scenario.
- [ ] Added original, redacted evidence.
- [ ] Completed the lab log.

## Result

Summarise the tests you actually ran and explain what the results showed.
