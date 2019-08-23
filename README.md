# attacks
Samples of the attacks presented in our paper.
These not represent the full flows we demonstrated, but basic implementation of their main parts.
We do not publish here the URLs and technical details of specific vendors, as part of the responsible vulnerability disclosure process.

## Attack I - attack1.html

The attack will add a port forwarding rule in the router with internal IP of [ROUTER_INTERNAL_IP], which forwards traffic to the router's external IP address and port [EXT_PORT], to the internal IP address of [INT_HOST] to port [INT_PORT].

Please replace:
* [ROUTER_INTERNAL_IP] with the internal IP address of thr router.
* [ROUTER_UPNP_PORT] with the router's UPnP port.
* [UPNP_COMMAND_PATH] with the UPnP commands control path.
* [EXT_PORT] with the external port to use in the port forwarding rule to add.
* [INT_PORT] with the internal port to use in the port forwarding rule to add.
* [INT_HOST] with the internal IP to use in the port forwarding rule to add.

## Attack II - attack2.html

The attack will send a crafted HTTP request by the user (currently a POST one) with [DATA] in its body, to the IoT device's HTTP server with URL [IOT_WEBSERVER_URL].

Please replace:
* [IOT_WEBSERVER_URL] with the URL of the IoT URL to attack.
* [DATA] with the crafted mailcious body of the HTTP request.



 
