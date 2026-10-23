# Assignment 1: From a URL to a Web Page

When I enter a web address and press Enter, the browser checks whether it can reuse a cached copy and uses DNS to find the server's IP address. It connects to the server (using TLS for HTTPS) and sends an HTTP request. The server replies with a status and the requested files. The browser reads the HTML to build the page structure, reads CSS to work out its appearance, and may request images, fonts, and other files. It then calculates where each item belongs, paints the result on screen, and runs JavaScript if the page uses it.

## Stages to remember

1. Find the server with DNS.
2. Connect and request the page with HTTP or HTTPS.
3. Parse HTML and CSS and request linked resources.
4. Calculate layout, paint the page, and run any JavaScript.
