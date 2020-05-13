# ninja-starter-kit

## installation
brew install nmap
brew install tor
brew install proxychains-ng

# scripts

## ninja-nmap

much safer nmap because it bypasses tor network and proxychain4

# usage

## nmap

you can scan open ports or target server with:
```
sudo nmap -sS server [url]
```

you can disguise your MAC address (not recommended: please use it ONLY for your own website)
```
$ sudo nmap -sT -Pn --spoof-mac 00:00:5e:00:53:00 [Url]
```

## tor

tor app (non-browser-version: can be retrieved from homebrew/MacPorts) can be used with curl such as:

```
$ brew services start tor
$ curl --socks5-hostname 127.0.0.1:9050 [Url]
$ brew services stop tor
```
