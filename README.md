# mikrotik-renew-certs
Script to renew SSL Certs from Mikrotik Router

Note, it's using ipv6, if you're using ipv4, simply switch the # / comment at Line 40 vs Line 41.

Note, it uses the comment:  allow Let's Encrypt  to find and open the firewall rule which is set to open port 80
IPv6 -> Firewall -> Filter -> New -> Chain = Input , Protocol = TCP , Dest.Port = 80, action = accept , comment = allow Let's Encrypt
If you use Ipv4, then just create the Filter Input rule for Ipv4.

Also, it temporary open port 80, open www service ( you need to change the port on www service to something else, like 8080 for www in Ip -> Service).

The rest just read the script. 

If reading is too much, copy & paste the script to AI like Gemini , it will show you steps by steps.
