# Static Routing Lab

## 1. What did I want to do?

I wanted to configure the PCs and routers from scratch and make PC1 ping PC2 through the routers.

The main thing I wanted to practice was static routing and basic IP configuration.

## 2. What did I do?

I started by configuring the IP addresses and hostnames on the routers.

Then I configured the router interfaces and used `no shutdown` to bring them up.

I configured the IP address, subnet mask, and default gateway on the PCs.

After that, I added static routes on the routers so they could reach the other networks.

I checked the interfaces with `show ip interface brief` and checked the routing tables with `show ip route`.

## 3. What happened?

At first, the routers were working and the static routes were configured correctly, but PC1 could not ping PC2.

I checked the configuration and found that I had forgotten to set the default gateway on the PCs.

After adding the correct gateways, I tested the connection again and PC1 was able to ping PC2 successfully.

## 4. Where did I make a mistake?

I forgot to configure the default gateway on the PCs.

The router configuration and static routes were fine, but without a default gateway, the PCs could not send traffic to networks outside their own network.

## 5. What did I learn?

I learned how to configure routers and PCs from scratch and how static routes are used to connect different networks.

I also understood better why the default gateway is important on a PC.

I practiced using `show ip interface brief`, `show ip route`, and `ping` to check if everything was working.