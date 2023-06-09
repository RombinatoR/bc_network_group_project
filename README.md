# bc_network_group_project

BeCode Network Module - Network Group Project

## Guidelines

With a team of 4, we had 4 days to establish a network plan in Cisco Packet Tracer.

The network must have :
- An AD server, DNS.
- A DHCP server.
- A DMZ (firewall, proxy).
- A storage server (iscsi).
- 4 Sectors :
    - 1 Management, secretariat: 5 posts
    - 2 Study : 8 posts.
    - 3 Production : 10 posts.
    - 4 Support (2 sectors): 30 posts per sector.

The plan had to be as complete as possible. It had include the IP address, the type of connection used, the number of switches etc...

## Team

- [Axel](https://github.com/Crucius96)
- [Nicolay](https://github.com/yadrychnikovNicolay)
- [Stéphane](https://github.com/RombinatoR)
- [Wouter](https://github.com/Hyamoto)

## Setups

We established 2 different plans, one where the network would have switches as its central part and the other where routers are setup in OSPF.

### Switch Network

After setting up all the workstations in their allocated sectors, we connected all the sectors to a quadruple switch network in the middle, acting as a core. (triple switch outside - one main switch inside)

Every sector switch connects to all 3 outer core switches, thus enabling redundancy and allowing the network to work even if a switch was to go down.

We then added a server zone and set up FTP, DNS, DHCP and AD servers. (AD was added per request of the exercice but we did not manage to make it work)

After the basic network was ready and the sectors interconnected, we set a connection from the inner core switch to a firewall, allowing us to start connecting our network to the outside world.

We connect the firewall to the DMZ with a Web Server inside and to a router leading the Cloud.

You can find the network plan(.pkt) in the newtorks folder, under the name "switchNetwork"

![switch network plan](./images/etwork-project-switches.png)

### Router Network

TODO TODO TODO TODO TODO TODO TODO TODO

![router network plan](./images/network-project-routers.png)

## Last Step

The last step of the group project was to present said project as a collective in a 5 minutes time limit. Having 2 projects we split the presentation time for each one of them to 2 minutes and a half.
