# mini_proxy_pro
I created a portable proxy for android (mini_proxy_pro.py).With this tool we can intercept the requests from any website.





# Mini Proxy Pro (HTTP & HTTPS Intercepting Proxy)

A lightweight, multi-threaded Python-based HTTP and HTTPS intercepting proxy server designed for local network debugging, request inspection, and educational security research.

---

## Features

* **HTTP & HTTPS Support:** Handles standard GET/POST HTTP requests as well as encrypted HTTPS traffic using HTTP `CONNECT` tunneling.
* **Multi-Threaded Architecture:** Utilizes Python threading to handle multiple concurrent client connections smoothly.
* **Real-Time Request Interception:** Captures and prints incoming request headers and targets directly to the console with clean ANSI color coding.
* **Lightweight & Portable:** Built using native Python libraries (`socket`, `select`, `threading`), requiring zero external dependencies or heavy installations.

---

## Prerequisites

Make sure you have **Python 3.x** installed on your system. No external pip packages are required.

---

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ishfaq0914/mini_proxy_pro.git

   git pull
  cd mini_proxy_pro



   
##  Run the proxy script:



python mini_proxy.py




Configure your browser/client:
Set your system or browser proxy settings to point to 127.0.0.1 on port 8080.



How It Works
HTTP Requests: Intercepts plain-text HTTP traffic, extracts target host and port headers, opens a socket connection to the destination server, forwards the request, and relays the response back to the client.
HTTPS Requests (CONNECT Method): Intercepts HTTPS tunneling handshakes, establishes a TCP tunnel between the client and the target server using select, and allows secure encrypted data streams to pass through.
Disclaimer
This tool is created strictly for educational purposes, local debugging, and authorized security assessments. Do not use it on networks or systems without explicit permission.
