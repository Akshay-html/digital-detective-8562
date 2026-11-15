# Mission 07 - How computers communicate

## 1. Task / objective

AI-assisted draft: explain network concepts, record a safe connectivity/DNS observation, and describe how a website request travels. Rephrase the concept descriptions in your own words.

## 2. Work completed

### Network concepts

| Concept | Short explanation | Example |
|---|---|---|
| LAN | Network covering a small local area. | Home Wi-Fi network. |
| MAN | Network covering a city or large campus. | Campus network linking buildings. |
| WAN | Network spanning large geographic areas. | The Internet. |
| DNS | Looks up an IP address for a domain name. | Resolves `example.com`. |
| Router | Forwards data between networks. | Home router connects devices to an ISP. |
| Protocol | Agreed rules for exchanging data. | HTTPS for secure web traffic. |
| Packet switching | Sends data as separate packets that can be routed. | Web page data travels in packets. |
| Client-server | A client requests a service; a server responds. | Browser requests a page from a web server. |

### Safe observations

- `ping -c 4 example.com`: 4 packets sent, 4 received, 0% packet loss during this check.
- `nslookup example.com`: DNS returned two public addresses. Only the domain and result were recorded; no personal IP or Wi-Fi details were included.
- A connectivity test checks whether a host responds over the network. A DNS lookup reports the address records currently associated with a name. DNS lets a browser use a readable site name instead of requiring a person to enter an IP address.

### What happens when a website opens (6 steps)

1. The user enters a site name; the browser acts as the client.
2. DNS looks up the server's network address for that name.
3. The device sends packets through its local network and router toward the server.
4. The client and server use network protocols (for example, HTTPS) to communicate.
5. The server processes the request and sends page data back in packets.
6. The browser receives the response and displays the page.

## 3. Commands / tools used

`ping -c 4 example.com` tested reachability; `nslookup example.com` queried DNS. The output depended on the current network and time.

## 4. My understanding

Reference note: DNS finds an address for a domain, routers forward packets between networks, and protocols define how the client and server exchange requests and responses. Rewrite in your own words.

## 5. Difficulties faced

No error occurred; the example host responded to all four connectivity checks.

## 6. How I resolved them

Not applicable.

## 7. Evidence / files

This README records the privacy-safe observations. The DNS server address and any personal network details are omitted.

## 8. Commit details

Commit message: `Explain networking concepts and website communication`.
