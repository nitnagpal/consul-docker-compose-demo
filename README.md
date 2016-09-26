# consul-docker-compose-demo
For Doing a Local Deploy:

1. git clone repo
2. cd to dir
3. docker-compose up
4. docker-compose have some issue with setting DNS 
   https://github.com/docker/compose/issues/2847
   Manually set the DNS in webapp containers in /etc/resolv.conf 
   from
      nameserver 127.0.0.11
   to
      nameserver 172.19.0.1   # or to what ever IP port 53 is mapped to 
      
Reference Links: 
http://howtocookmicroservices.com/docker-compose/ 
https://sreeninet.wordpress.com/2016/04/17/service-discovery-with-consul/ 
http://progrium.com/blog/2014/08/20/consul-service-discovery-with-docker/ 
