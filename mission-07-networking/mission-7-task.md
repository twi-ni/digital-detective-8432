# Mission 7 – How Computers Communicate

## Task 7.1 – Explain Network Concepts

In this task, I learned about some basic networking concepts and how computers use networks to communicate with each other. A network basically connects different devices so they can share information and resources.

| Concept | Explanation | Example |
|---|---|---|
| LAN (Local Area Network) | A network that connects devices in a small area, like a home, office or lab. | Devices connected to the same home Wi-Fi. |
| MAN (Metropolitan Area Network) | A network that covers a bigger area, like a city or a large campus. | A network connecting different buildings in a university. |
| WAN (Wide Area Network) | A network that connects devices over large distances. | The Internet. |
| DNS (Domain Name System) | DNS changes website names into IP addresses so computers can find websites. | Finding the IP address of `google.com`. |
| Router | A router connects networks and helps send data to the right place. | A Wi-Fi router connecting phones and laptops to the Internet. |
| Protocol | A protocol is a set of rules that devices follow while communicating. | HTTP and HTTPS are used when opening websites. |
| Packet Switching | It means breaking data into smaller parts called packets and sending them over a network. | Sending a photo over the Internet. |
| Client-Server | It is a way of communication where one device asks for something and another device provides it. | A browser requesting a webpage from a server. |

### What I Understood

I learned that different networks are used for different areas, from a small home network to the Internet. DNS helps us open websites without having to remember their IP addresses. Routers help move data between networks, and protocols make sure devices follow the right rules while communicating. I also learned how data is sent in small packets and how clients and servers work together when we open a website.

## Task 7.2 – Observe Network Information

In this task, I used Terminal to check my internet connection and find the IP address of a website.

### 1. Connectivity Test
Command used:
ping -c 4 google.com
I used this command to check if my computer could connect to `google.com`. It sent 4 packets to the website and showed the replies and the time taken.
This test helps us check if our computer can reach a website and whether there are any connection problems.

### 2. DNS Lookup
Command used:
nslookup example.com
I used this command to find the IP address of `google.com`.
The output showed the DNS server used and the IP address linked to the website.

### 3. Role of DNS
DNS stands for Domain Name System. It converts website names into IP addresses.
For example, when we type a website name in our browser, DNS helps find its IP address so our computer can connect to the correct server.

### What I Understood
I understood that `ping` is used to check if a website can be reached, while `nslookup` is used to find its IP address. Both commands help us understand how computers connect to websites.

## Task 7.3 – What Happens When You Open a Website?

When we open a website, a few things happen in the background to load the page. The steps are:

1. Enter the website address: First, we type a website name like `www.google.com` in our browser.

2. DNS finds the IP address: DNS finds the IP address linked to the website name so our computer knows where to connect.

3. Connect to the server: Our computer connects to the website's server through the internet. The router helps send the data.

4. Browser sends a request: The browser sends a request to the server using HTTPS. Here, the browser acts as the client.

5. Server receives the request: The server gets the request and prepares the webpage.

6. Server sends the data back: The server sends the webpage data back to our computer.

7. Website opens: Finally, the browser loads the data and shows the website on our screen.

### What I Understood

I understood that many things happen in the background when we open a website. DNS helps find the website's IP address and the browser and server communicate with each other to load the page.