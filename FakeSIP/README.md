# FakeSIP

Disguise your UDP traffic as SIP protocol to evade DPI detection, using Netfilter Queue (NFQUEUE).

[[ 中文文档 ]](https://github.com/MikeWang000000/FakeSIP/wiki)


## Quick Start

```
按需添加伪装服务或添加payload.bin承载文件，根据实际网络情况逐渐调整跃点值大小直至“解除限速”。如果出现网络异常，关闭软件后重启飞牛os。受限于运营商及地区限制，该项目不保证有效解除网络限速。
```


## Usage

```
Usage: fakesip [options]

Interface Options:
  -a                 work on all network interfaces (ignores -i)
  -i <interface>     work on specified network interface

Payload Options:
  -b <file>          use UDP payload from binary file
  -u <uri>           use specified SIP URI

General Options:
  -0                 process inbound packets
  -1                 process outbound packets
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
