# IPScanner
Explodes a range of IPV4 addresses provided by the user, does a rDNS lookup on each IP. If the rDNS lookup returns data, the app sends an HTTP HEAD request to the IP, returns the status code, the IP's geolocation, headers if available, and HTML if the IP is a web server. It provides the user with a list of webservers, their HTML as a string, headers, and a basic WebView to see what the page looks like, and a MapKit view to see the IPs location.

# Bad coding practice
I was able to implement a Session Delegate that blindly trusts all SSL certificates, this is bad coding because it is insecure, and quite frankly I just wanted to see if it would work. If you would like more information on why bypassing SSL certificates is bad, check out this article (https://www.cs.utexas.edu/~shmat/shmat_ccs12.pdf). Basically, ATS wasn't letting me do what I wanted, so I went around it.

# Requirements
Xcode 13 beta or above, I'm using Version 13.1 (13A1030d) at the moment
