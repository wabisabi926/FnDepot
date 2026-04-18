# FakeHTTP

Obfuscate all your TCP connections into HTTP protocol, using Netfilter Queue (NFQUEUE).

[[ 中文文档 ]](https://github.com/MikeWang000000/FakeHTTP/wiki)


## Quick Start

```
⭐使用方法：按需添加伪装参数或添加payload.bin承载文件，根据实际网络情况逐渐调整跃点值大小直至“解除限速”。如果出现网络异常，关闭软件后重启飞牛os。受限于运营商及地区限制，该项目不保证有效解除网络限速。
```


## Usage

```
Usage: fakehttp [options]

Interface Options:
  -a                 work on all network interfaces (ignores -i)
  -i <interface>     work on specified network interface

Payload Options:
  -b <file>          use TCP payload from binary file
  -e <hostname>      hostname for HTTPS obfuscation
  -h <hostname>      hostname for HTTP obfuscation

General Options:
  -0                 process inbound connections
  -1                 process outbound connections
  -4                 process IPv4 connections
  -6                 process IPv6 connections
  -d                 run as a daemon
  -k                 kill the running process
  -s                 enable silent mode
  -w <file>          write log to <file> instead of stderr

Advanced Options:
  -f                 skip firewall rules
  -g                 disable hop count estimation
  -m <mark>          fwmark for bypassing the queue
  -n <number>        netfilter queue number
  -r <repeat>        duplicate generated packets for <repeat> times
  -t <ttl>           TTL for generated packets
  -x <mask>          set the mask for fwmark
  -y <pct>           raise TTL dynamically to <pct>% of estimated hops
  -z                 use iptables commands instead of nft

```


## License

GNU General Public License v3.0
