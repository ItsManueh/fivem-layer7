# FiveM / RedM Blocked Layer7 Vulnerability (DDoS Attack & Get information)

 The main cause of the attack is the information that FiveM gives you open to the public on the web by putting ip/players.json or ip/info.json this makes possible the vulnerability known as Layer7.

 It is possible to do a denial of service in just minutes leaving it unusable the server and the machine, it can get information from the server if the attacker wants it.

 That's why I would like to provide some config that you should put in your server.cfg.

 When you apply these configs on your server, if you want to check that the information is blocked, do not refresh the web ip/players.json several times because it is possible that the connection to your server will be blocked for a few minutes.

 You can also check in the famous CFX Finder bot to put your URL code and you will see that said information is completely blocked.

 At the first connection in the URL /players.json you will have the list of users with their ping but after a refresh you will have the message Nope. If you get Nope, everything is correct.
 
 ```
sv_endpointprivacy true

set sv_requestParanoia 3 

sv_forceIndirectListing true

sv_useDirectListing true
```

 I usually recommend that you put this configuration but this limits that the user does or does have to go through the discord to obtain the connect XXXXXX (Using F8 for the connect) using the FiveM URL code instead of the IP. 

 ```
sv_master1 "" - Put your server on Private

sets sv_pureLevel 1 - Block Modified Clients

sv_endpointPrivacy true - Block Endpoints from IP Externals

sv_forceIndirectListing true - Block Listing
```
