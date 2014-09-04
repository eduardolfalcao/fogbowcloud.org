Title: Reverse Tunnel
url: install-reverse-tunnel
save_as: install-reverse-tunnel.html
section: install
index: 5

# Reverse Tunnel

blablabla

## Install

To set up the reverse tunnel server, first, get the latest code from github.
```bash
git clone https://github.com/fogbow/fogbow-reverse-tunnel.git
```
Then, install it with Maven
```bash
mvn install
```

## Configure

After the installation, move the file ```reverse-tunnel.conf.example``` to ```reverse-tunnel.conf``` and edit its contents:

```bash
# Tunnel port for ssh
tunnel_port=2222

# Port for requests HTTP
http_port=2223

# Range for external ports
external_port_range=40000:50000

# Path for host key file
host_key_path=hostkey.ser

```

## Run

To start the reverse tunnel server, run the start-tunnel-server.

```bash
./start-tunnel-server
```