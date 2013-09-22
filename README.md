# Go TCP Proxy
This simple application is a TCP proxy server written in golang. 

By default the server proxies from localhost:80 to localhost:8000 and has a maximum number of active connections (connections connected to the hidden server) of 25.

## Usage Examples
- Forwarding all requests from localhost:80 (default) to localhost:3000

```
./proxy -to localhost:3000 
```

- Forwarding all requests from localhost:10000 to somedomain.com:80

```
./proxy -from localhost:10000 -to somedomain.com:80
```

- Changing the number of maximum active connections to 300

```
./proxy -c 300
```