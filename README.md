# attacks
Samples of the attacks presented in our paper.
These not represent the full flows we demonstrated, but basic implementation of their main parts.
We do not publish here the URLs and technical details of specific vendors, as part of the responsible vulnerability disclosure process.

## Attack I - [attack1.html](https://github.com/INP-attacks/attacks/blob/master/attack1.html)  

The attack will add a port forwarding rule in the router with internal IP of [ROUTER_INTERNAL_IP], which forwards traffic to the router's external IP address and port [EXT_PORT], to the internal IP address of [INT_HOST] to port [INT_PORT].

Please replace:
* [ROUTER_INTERNAL_IP] with the internal IP address of thr router.
* [ROUTER_UPNP_PORT] with the router's UPnP port.
* [UPNP_COMMAND_PATH] with the UPnP commands control path.
* [EXT_PORT] with the external port to use in the port forwarding rule to add.
* [INT_PORT] with the internal port to use in the port forwarding rule to add.
* [INT_HOST] with the internal IP to use in the port forwarding rule to add.

### Scanning for an HTTP endpoint - [upnpPortChecker.html](https://github.com/INP-attacks/attacks/blob/master/attack1.html)
In Appendix A, we show how we can expand Attack I, to work with routers whouse UPnP port is randomized. As an example, we show here a HTML page which scans a specific HTTP endpoint (which can of course be a UPnP server), and sends thes scan's result to an external server of the attacker.

* [ROUTER_INTERNAL_URL] with the internal IP of the device to scan.
* [PORT_TO_CHECK] with the TCP port to scan if it is of an HTTP endpoint.
* [ATTACKER_SERVER] with the IP of an attacker's server, to send the result to.


## Attack II - [attack2.html](https://github.com/INP-attacks/attacks/blob/master/attack2.html)

The attack will send a crafted HTTP request by the user (currently a POST one) with [DATA] in its body, to the IoT device's HTTP server with URL [IOT_WEBSERVER_URL].

Please replace:
* [IOT_WEBSERVER_URL] with the URL of the IoT URL to attack.
* [DATA] with the crafted mailcious body of the HTTP request.

## Attack III - [attack3.html](https://github.com/INP-attacks/attacks/blob/master/attack3.html)

The attack will use HTML form to login to the router with URL [ROUTER_LOGIN_LOCATION], with username [LOGIN_USERNAME] and password [LOGIN_PASSWORD]. Then it will redirect the user to the AP List page in URL [ROUTER_AP_LIST_LOCATION].

Please replace:
* [ROUTER_AP_LIST_LOCATION] with the URL of the router's AP List page.
* [ROUTER_LOGIN_LOCATION] with the URL of the router's Login page.
* [LOGIN_USERNAME_VAR] with the variable name of the username in the router's login form.
* [LOGIN_USERNAME] with the username to login with.
* [LOGIN_PASSWORD_VAR] with the variable name of the password in the router's login form.
* [LOGIN_PASSWORD] with the username to login with.




 
