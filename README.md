# V2RayAggregator


[![Collect](https://github.com/mahdibland/SSAggregator/actions/workflows/Collector.yml/badge.svg)](https://github.com/mahdibland/SSAggregator/actions/workflows/Collector.yml) [![Airport Collect](https://github.com/mahdibland/SSAggregator/actions/workflows/Airport_Collector.yml/badge.svg)](https://github.com/mahdibland/SSAggregator/actions/workflows/Airport_Collector.yml)

## Quick Note & Updates
🔴 ~~This project is still under maintance. so don't use it until further announcement cause there is a chance you will get errors while updating the nodes, etc.~~  

🟢 11/1/2022: from now you can use this project. also readme file updated with the recent changes so you can find out which file to use.

## Introduction

The automation functions of this repository are all implemented based on `GitHub Actions`

Test the speed of each free node pool on the network and the nodes shared by bloggers to screen out relatively stable and high-speed nodes, and then import them into the warehouse for sharing records.

The speed measurement function is implemented in the `GitHub Actions` environment using [LiteSpeedTest](https://github.com/xxf098/LiteSpeedTest), so there are many nodes in the United States, which cannot well represent the node availability in the domestic network environment.

## Features
- Lots of sources 😯
- Remove all duplicate nodes 🤤
- Providing nodes in major formats (YAML, clash, v2ray, base64) 🦋
- No additional conversion to prevent breaking the nodes 🌿
- Filtering best nodes by testing them and sorting them based on their average speed 🍀

## Recent Todos
- [x] ~~Fix region based lite speed test (mainly EU)~~ 👀
- [x] Fix Sort Based on the Avg Speed 👀
- [x] Update required softwares to latest version 👀
- [x] Fix sources that subconvertor unable to convert 👀
- [x] Add separate files & functions for airport 👀
- [x] Fix name (emoji+ip) for all log files 👀
- [x] Separate sub list for airports & other nodes 👀
- [x] Fixed clash template 👀
- [ ] Cleanup redundant files and functions (dev Branch) 🧲

## Visualizer

- Log Visualizer on Netlify 
> if you click on any node url it will copy to clipboard



|                  |             Link to Log              |
|:----------------:|:-----------------------------:|
|   Public Nodes   |   <a href="https://55292969231427515295.netlify.app/" target="_blank"><img src="https://i.ibb.co/g32RmJy/netlify.png" width="35"/></a>   |
|     Airport      |   <a href="https://55292969231427515295.netlify.app?type=airport" target="_blank"><img src="https://i.ibb.co/g32RmJy/netlify.png" width="35"/></a>   |

## Instructions & Usage

### Tips
- If you see an IP repeated more than once it's usually because of the different ports.
- (Group 2) Some free airports only provide 1GB of traffic or have limited time to use that's why I update the airport node every 2 hours. so if you want to use them set the auto-update option on your client to get fresh nodes.
- (Group 1) Other public nodes are more stable and will be updated every 12 hours.
- Depending on your internet provider and location, some nodes might not work.


### Ready to import (200 filtered nodes)
> Just import the following subscription link into the corresponding client. Use a client that atleast support ss + ssr + vmess + trojan.

Nodes filtered using speedtest measurement will be stored in following files:  

* Group 1 (Contains free public nodes)
- [Base64](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity)
- [Mixed](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.yml)

* Group 2 (Contains only free airports)
- [Base64](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/EternityAir)
- [Mixed](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/EternityAir.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/EternityAir.yml)

### For Local Testing (all nodes)
> Only for local testing because the number of nodes is too high and your client will crash if you import them  

All of the nodes merged together will be stored in following files:  

* Group 1 (Contains free public nodes)
- [Base64](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge_base64.txt)
- [Mixed](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge_yaml.yml)

* Group 2 (Contains only free airports)
- [Base64](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/airport_merge_base64.txt)
- [Mixed](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/airport_sub_merge.txt)
- [Clash](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/airport_merge_yaml.yml)

### Manual Subs Conversion
- If your client does not support the formats that provided here use below services to convert them to your client format (like surfboard)
> Services for online sub conversion: 
- [sub-web-modify](https://sub.v1.mk/)
- [bianyuan](https://bianyuan.xyz/)  

- **If you don't like the groups and rules that are already set, you can simply use bianyuan API like this::**  
> don't use this API for your personal airport subs! Pls run the subconverter locally
```
https://pub-api-1.bianyuan.xyz/sub?target=(OutputFormat)&url=(SubUrl)&insert=false

For Example:
(OutputFormat) = clash
(SubUrl) = https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.yml

https://pub-api-1.bianyuan.xyz/sub?target=clash&url=https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/Eternity.yml&insert=false

Now you can use the link above to import the subs into your client
```

<br/>

## Node Information

### high-speed node
high-speed node quantity: `200`

<details>
    trojan://dfbf0d67-f03d-4184-a224-c2d64a571f99@s1.hass.win:12340?allowInsecure=1&sni=static.dingtalk.com#%F0%9F%87%BA%F0%9F%87%B8US-147.182.224.102-12778
    vmess://ewogICAgImFkZCI6ICJobXMxODIuZ2x3ZWlkZi5zYnMiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJnbHdlaWRmLnNicyIsCiAgICAiaWQiOiAiNzYyMjFiZmItZTkyZi00ZTgwLTgxYzUtNmZlNDhmNTBhYzBiIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmt3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIxLjE1LjIxMi0wMTkxIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiZ2x3ZWlkZi5zYnMiCn0=
    vmess://ewogICAgImFkZCI6ICJobXMwNy54Zml4ZWRmbG9hdC5jZmQiLAogICAgImFpZCI6IDEsCiAgICAiaG9zdCI6ICJhZnJobXMwNy54Zml4ZWRmbG9hdC5jZmQiLAogICAgImlkIjogImExNjU1ZjUxLTFlMjAtNGE5Mi04YTExLWI3Y2EzMGE3YTM1MyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9saW5rd3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS43NC4yMzktMTQ1NiIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJobXMyNC5pdmlkZW9zLnNicyIsCiAgICAiYWlkIjogMSwKICAgICJob3N0IjogIml2aWRlb3Muc2JzIiwKICAgICJpZCI6ICI0NDFkYTM0Mi1jZTkwLTQ0MWUtYmZmOS1kMmNlYjU1ZTY4Y2EiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlua3dzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjEuNDYuMTIxLTE0NTIiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@212.102.47.198:443#%F0%9F%87%BA%F0%9F%87%B8US-212.102.47.198-0790
    vmess://ewogICAgImFkZCI6ICJsaW5kZTA2LmluZGlhdmlkZW8uc2JzIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibGluZGUwNi5pbmRpYXZpZGVvLnNicyIsCiAgICAiaWQiOiAiZWRiYjEwNTktMTYzMy00MjcxLWI2NmUtZWQ0ZmJhNDdhMWJmIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmt3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIxLjE1LjM2LTAxODQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJsaW5kZTA2LmluZGlhdmlkZW8uc2JzIgp9
    vmess://ewogICAgImFkZCI6ICIxMDQuMjEuNzMuMTQiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ5YWdob29iNTVmcmVlbm9kZXMucmVwYWNvNjk0Mzc0MDMud29ya2Vycy5kZXYiLAogICAgImlkIjogIjQ1ZjYzZTkyLWY3ODItNGNhYy04NGI4LWU2MWNiNWE1YmZkMCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9hZGVuYzM1LmZpeGVkbGZvYXQudG9wL2xpbmt3cyIsCiAgICAicG9ydCI6IDg4ODAsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS43My4xNC0xNzE1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@156.146.38.163:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.163-3465
    ssr://MTU2LjE0Ni4zOC4xNjM6NDQzOm9yaWdpbjphZXMtMTI4LWNmYjpwbGFpbjpjMmhoWkc5M2MyOWphM009Lz9vYmZzcGFyYW09JnJlbWFya3M9OEolMkJIdXZDZmg3aFZVeTB4TlRZdU1UUTJMak00TGpFMk15MDVNRFEzJnByb3RvcGFyYW09
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@156.146.38.163:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.163-0256
    vmess://ewogICAgImFkZCI6ICIxMDQuMjEuMzAuMjU0IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibmluYS5ib25kIiwKICAgICJpZCI6ICIwM2ZjYzYxOC1iOTNkLTY3OTYtNmFlZC04YTM4Yzk3NWQ1ODEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlua3Z3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIxLjMwLjI1NC01MzU4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAibmluYS5ib25kIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpxR2ptSThXUWxGMHRmaERia0xxR2RO@passconf.xyz:8080#%F0%9F%87%BA%F0%9F%87%B8US-172.233.142.162-0802
    vmess://ewogICAgImFkZCI6ICJuaW5hLmJvbmQiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJuaW5hLmJvbmQiLAogICAgImlkIjogIjAzZmNjNjE4LWI5M2QtNjc5Ni02YWVkLThhMzhjOTc1ZDU4MSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9saW5rdndzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjEuMzAuMjU0LTAxOTQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IGZhbHNlLAogICAgInNuaSI6ICJuaW5hLmJvbmQiCn0=
    vmess://ewogICAgImFkZCI6ICIxMjkuMTQ2LjExMy4yNTQiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogImQ1M2IzOWUyLTkyNWUtNDViNi05Mzg5LTQ2YjlmYTk1ODc4YiIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiA0MzEyMSwKICAgICJwcyI6ICLwn4e68J+HuFVTLTEyOS4xNDYuMTEzLjI1NC0wNzc5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTplemVzQlhlc2YzUktCQ3AxdnFLdUl4@beeconf.xyz:8080#%F0%9F%87%BA%F0%9F%87%B8US-172.234.30.123-0765
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTplemVzQlhlc2YzUktCQ3AxdnFLdUl4@beeconf.xyz:8080#%F0%9F%87%BA%F0%9F%87%B8US-172.234.30.123-3483
    vmess://ewogICAgImFkZCI6ICIxNzIuNjcuMTMxLjEwOCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImdsd2VpZGYuY2ZkIiwKICAgICJpZCI6ICIxMDUyZjI0ZS03YjA5LTQ1ZWItYjBjNS1kODU4ZWIxMjQxOTIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlua3dzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzIuNjcuMTMxLjEwOC0xOTkzIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6MjE3MGY4@45.55.2.232:14293#%F0%9F%87%BA%F0%9F%87%B8US-45.55.2.232-0812
    ss://YWVzLTEyOC1nY206QmlhL1RlbGVncmFtL1YycmF5X0FscGhhL2pvaW5TSG9KdVRSRUhYcUIyRVFhd1ZNKzdVRVdFUmw0PQ==@5.78.63.157:2096#%F0%9F%87%BA%F0%9F%87%B8US-5.78.63.157-9092
    ss://eGNoYWNoYTIwLWlldGYtcG9seTEzMDU6QmlhL1RlbGVncmFtL1YycmF5X0FscGhhL2pvaW5TSG9KdVRSRUhYcVEyRVFQQkVNKzRwYldFUmw0PQ==@5.78.63.157:2087#%F0%9F%87%BA%F0%9F%87%B8US-5.78.63.157-9093
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpCaWEvVGVsZWdyYW0vVjJyYXlfQWxwaGEvam9pblNIb0p1VFJFSFhxUTJFUWF3Vk0rNHBiV0VSbDQ9@5.78.63.157:443#%F0%9F%87%BA%F0%9F%87%B8US-5.78.63.157-9091
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpSOVhjNGRIWEd2M2M=@205.134.180.143:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.143-7806
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTo5QnZrdzVhdXBOeTg=@205.134.180.147:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.147-0826
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpoZ0xDZ2ZMUmdCNmQ=@205.134.180.145:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.145-0791
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTo1Y3A5WjNpV25KWjI=@205.134.180.151:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.151-0771
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpnMTNTN2RvWGFyMEE=@205.134.180.137:443#%F0%9F%87%BA%F0%9F%87%B8US-205.134.180.137-0803
    trojan://telegram-id-directvpn@3.20.230.45:22222?security=tls&sni=trj.rollingnext.co.uk#%F0%9F%87%BA%F0%9F%87%B8US-3.20.230.45-0162
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpINmNTVGY4dkRiVkgxY3BuckF4Rmoy@18.218.239.120:36326#%F0%9F%87%BA%F0%9F%87%B8US-18.218.239.120-0810
    vmess://ewogICAgImFkZCI6ICIyMDYuMjM4LjIzNi4zNiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIm15c2FuMi5qYXF1YXkyMi53b3JrZXJzLmRldiIsCiAgICAiaWQiOiAiZjU4NGRlMTUtMjAzNC00MTcwLWE3MjMtZjQ4YzJiYWU1ZTBmIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2FmcmhtczE2di5iZXN0eHJheS5idXp6L2xpbmt3cyIsCiAgICAicG9ydCI6IDIwNTIsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0yMDYuMjM4LjIzNi4zNi0wMTg3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxMzIuMTQ1LjEzMi4yMjciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjkzODQ1YjUwLTI2ZjYtNDIwMy1mNWFkLTRkMjMxZDRlOGY0NSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAzNzEyMSwKICAgICJwcyI6ICLwn4e68J+HuFVTLTEzMi4xNDUuMTMyLjIyNy0wMzg3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJnbHdlaWRmLmNmZCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImdsd2VpZGYuY2ZkIiwKICAgICJpZCI6ICIxMDUyZjI0ZS03YjA5LTQ1ZWItYjBjNS1kODU4ZWIxMjQxOTIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlua3dzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzIuNjcuMTMxLjEwOC0xNDU3IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://6c609341-9919-417c-b4c4-b8dc84057072@us3-full.privateip.net:443?security=tls#%F0%9F%87%BA%F0%9F%87%B8US-165.227.221.123-0761
    trojan://xxoo@us.blazeppn.info:443?security=tls#%F0%9F%87%BA%F0%9F%87%B8US-138.197.5.103-7868
    vmess://ewogICAgImFkZCI6ICIxNDIuMTcxLjIzNy4yMTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAid3d3LjIzMTY4NDk5Lnh5eiIsCiAgICAiaWQiOiAiNDE4MDQ4YWYtYTI5My00Yjk5LTliMGMtOThjYTM1ODBkZDI0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3BhdGgvMjIxMzEyMjgxMDA5IiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtMTQyLjE3MS4yMzcuMjE0LTIwNTkiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIwOGRmZGU1MS04YzVkLTQxNjAtODczMi0wNzQ1NTA3Y2ZkNWIuY2xvdWRmbGFyZS1nYXRld2F5LmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIm1pa2FzYS5lcmVueWVhZ2VyLmNsb3VkbnMuYml6IiwKICAgICJpZCI6ICI3NjIyMWJmYi1lOTJmLTRlODAtODFjNS02ZmU0OGY1MGFjMGIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZ2x3ZWlkZi5zYnMvbGlua3dzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNjIuMTU5LjM2LjIwLTE5MTYiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1nY206MzFMZFloUDhBZQ==@45.58.39.13:58428#%F0%9F%87%BA%F0%9F%87%B8US-45.58.39.13-0509
    trojan://892e4ff3-f8bb-42ac-9bd5-e103f235fc78@us03.333210.xyz:40000?security=tls&sni=400567.xyz#%F0%9F%87%BA%F0%9F%87%B8US-100.20.63.113-9190
    vmess://ewogICAgImFkZCI6ICI2Ni4xODEuMzMuMTA4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI5ZjA5NmM3MC00NzhhLTRmZWYtYjI5Zi0wZjE0ZDZhMDY1ODMiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvYT9lZD0yMDQ4IiwKICAgICJwb3J0IjogMjI2NjYsCiAgICAicHMiOiAi8J+HuvCfh7hVUy02Ni4xODEuMzMuMTA4LTQwOTIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICI4MC45Mi4yMDUuMTEyIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0YzkwYmE3NS0yMzBiLTRmOGItYmJmZi04ZWZhMGViMDQxNWYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtODAuOTIuMjA1LjExMi0wODE5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@13.231.78.35:443#%F0%9F%87%AF%F0%9F%87%B5JP-13.231.78.35-9037
    trojan://892e4ff3-f8bb-42ac-9bd5-e103f235fc78@jp05.333210.xyz:40000?security=tls&sni=400567.xyz#%F0%9F%87%AF%F0%9F%87%B5JP-54.64.207.117-9064
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@18.182.4.118:443#%F0%9F%87%AF%F0%9F%87%B5JP-18.182.4.118-5387
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@18.179.13.191:443#%F0%9F%87%AF%F0%9F%87%B5JP-18.179.13.191-5385
    trojan://94744160-abe9-44ca-b085-0f6994e1944e@a22.zgc.su:567?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-52.195.13.70-2134
    trojan://94744160-abe9-44ca-b085-0f6994e1944e@18.180.193.232:567?security=tls&sni=a4.zgc.su#%F0%9F%87%AF%F0%9F%87%B5JP-18.180.193.232-0186
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@54.64.31.75:443#%F0%9F%87%AF%F0%9F%87%B5JP-54.64.31.75-5384
    trojan://842b5f9dd11e458d8613c907c4cc5723@38.207.136.202:443?security=tls&sni=www.gpt123.one#%F0%9F%87%AF%F0%9F%87%B5JP-38.207.136.202-0196
    trojan://94744160-abe9-44ca-b085-0f6994e1944e@a4.zgc.su:567?security=tls#%F0%9F%87%AF%F0%9F%87%B5JP-18.180.193.232-0830
    trojan://94744160-abe9-44ca-b085-0f6994e1944e@52.195.13.70:567?security=tls&sni=a22.zgc.su#%F0%9F%87%AF%F0%9F%87%B5JP-52.195.13.70-0171
    vmess://ewogICAgImFkZCI6ICIxMDQuMTguMjAyLjI1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImVyZmFubmV3ZnJlZW5vZGVzLnZkbW1zd3l6bXppZ29udm5qazQ0My53b3JrZXJzLmRldiIsCiAgICAiaWQiOiAiMDNmY2M2MTgtYjkzZC02Nzk2LTZhZWQtOGEzOGM5NzVkNTgxIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL25pbmEuYm9uZC9saW5rdndzIiwKICAgICJwb3J0IjogMjA4MiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE4LjIwMi4yNTAtMTk3NSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ssr://anAtYW00OC02LmVxbm9kZS5uZXQ6ODA4MTpvcmlnaW46YWVzLTI1Ni1jZmI6dGxzMS4yX3RpY2tldF9hdXRoOlpVRnZhMkpoUkU0Mi8/b2Jmc3BhcmFtPSZyZW1hcmtzPThKJTJCSHIlMkZDZmg3VktVQzAwTXk0eU1EY3VNVFF6TGpRdE1EZ3lNdyUzRCUzRCZwcm90b3BhcmFtPQ==
    ss://YWVzLTI1Ni1jZmI6cXdlclJFV1FAQA==@p229.panda004.net:57428#%F0%9F%87%B0%F0%9F%87%B7KR-125.141.26.8-5413
    ss://YWVzLTI1Ni1jZmI6cXdlclJFV1FAQA==@p232.panda004.net:4398#%F0%9F%87%B0%F0%9F%87%B7KR-221.150.109.82-5418
    trojan://842b5f9dd11e458d8613c907c4cc5723@104.160.18.251:443?security=tls&sni=www.gpt123.one#%F0%9F%87%BA%F0%9F%87%B8US-104.160.18.251-0175
    vmess://ewogICAgImFkZCI6ICIxNTIuNjcuMjE4LjM4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTUyLjY3LjIxOC4zOCIsCiAgICAiaWQiOiAiYjVlOTQ4MGEtYjdhYS00MGE0LWY5YTctNTI5OWI1ZTM2M2I0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE1Mi42Ny4yMTguMzgtODA0MyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://telegram-id-directvpn@185.48.122.94:22222?security=tls&sni=trojan.miwan.co.uk#%F0%9F%87%AE%F0%9F%87%AAIE-185.48.122.94-0190
    vmess://ewogICAgImFkZCI6ICJrZWxsaWUubWFrZXVwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAia2VsbGllLm1ha2V1cCIsCiAgICAiaWQiOiAiMDNmY2M2MTgtYjkzZC02Nzk2LTZhZWQtOGEzOGM5NzVkNTgxIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2xpbmt2d3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS40NC42NC0xODYzIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.193:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.193-0808
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.81:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.81-0828
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.79:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.79-0878
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.80:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.80-0815
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.194:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.194-0254
    trojan://telegram-id-directvpn@18.169.174.246:22222?security=tls&sni=trojan.miwan.co.uk#%F0%9F%87%AC%F0%9F%87%A7GB-18.169.174.246-0181
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.197:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.197-0820
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.195:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.195-0778
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.78:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.78-0843
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.198:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.198-0821
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@77.72.5.150:989#%F0%9F%87%AC%F0%9F%87%A7GB-77.72.5.150-0776
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.196:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.196-0897
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp1Zk1iWWFSTmZtT3pGZkF6NTVDaHcz@178.79.187.120:80#%F0%9F%87%AC%F0%9F%87%A7GB-178.79.187.120-0804
    vmess://ewogICAgImFkZCI6ICJtaW5nMi5raXdpcmVpY2guY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibWluZzIua2l3aXJlaWNoLmNvbSIsCiAgICAiaWQiOiAiMThlNWY0MGYtYmRhNi00YzE1LTkzMzQtZTg3Y2RhNjA0N2FmIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3JheSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTcyLjY3LjEzMi4xNS0xMTA0NCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNzIuOTkuMTkwLjEwOSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMDNmY2M2MTgtYjkzZC02Nzk2LTZhZWQtOGEzOGM5NzVkNTgxIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAibGlua3Z3cyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4es8J+Hp0dCLTE3Mi45OS4xOTAuMTA5LTIxMjEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpCb2cwRUxtTU05RFN4RGRR@series-a2-me.samanehha.co:443#%F0%9F%87%AC%F0%9F%87%A7GB-13.41.38.181-0807
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp1MTdUM0J2cFlhYWl1VzJj@series-a2-mec.samanehha.co:443#%F0%9F%87%AC%F0%9F%87%A7GB-3.10.242.58-0837
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpXNzRYRkFMTEx1dzZtNUlB@series-a1.samanehha.co:443#%F0%9F%87%AC%F0%9F%87%A7GB-18.170.152.153-3726
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTptcHMzRndtRGpMcldhT1Zn@series-a2.samanehha.co:443#%F0%9F%87%AC%F0%9F%87%A7GB-18.170.152.153-5327
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@51.15.27.48:989#%F0%9F%87%AB%F0%9F%87%B7FR-51.15.27.48-0782
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTptcHMzRndtRGpMcldhT1Zn@13.42.146.210:443#%F0%9F%87%AC%F0%9F%87%A7GB-13.42.146.210-2109
    ssr://NTEuMTU5LjExMS4yMDg6OTg5Om9yaWdpbjphZXMtMjU2LWNmYjpwbGFpbjpaamhtTjJGRGVtTlFTMkp6Umpod013PT0vP29iZnNwYXJhbT0mcmVtYXJrcz04SiUyQkhxJTJGQ2ZoN2RHVWkwMU1TNHhOVGt1TVRFeExqSXdPQzA1TURReiZwcm90b3BhcmFtPQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpCb2cwRUxtTU05RFN4RGRR@Fast_2ray_Telchannelll.fast2rayy.eu.org:443#%F0%9F%87%AC%F0%9F%87%A7GB-13.41.38.181-3879
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@51.159.111.208:989#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.111.208-0784
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@195.154.185.174:989#%F0%9F%87%AB%F0%9F%87%B7FR-195.154.185.174-0817
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpCb2cwRUxtTU05RFN4RGRR@18.171.3.198:443#%F0%9F%87%AC%F0%9F%87%A7GB-18.171.3.198-2105
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpCb2cwRUxtTU05RFN4RGRR@jseyu.arvancode.eu.Org:443#%F0%9F%87%AC%F0%9F%87%A7GB-13.41.38.181-0832
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@109.201.152.181:443#%F0%9F%87%B3%F0%9F%87%B1NL-109.201.152.181-0777
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@51.159.111.208:989#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.111.208-0780
    trojan://telegram-id-directvpn@15.236.110.253:22222?security=tls&sni=trj.rollingnext.co.uk#%F0%9F%87%AB%F0%9F%87%B7FR-15.236.110.253-3714
    trojan://telegram-id-directvpn@15.236.56.28:22222?security=tls&sni=trojan.miwan.co.uk#%F0%9F%87%AB%F0%9F%87%B7FR-15.236.56.28-0167
    trojan://telegram-id-privatevpns@13.37.22.159:22222?security=tls&sni=trojan.miwan.co.uk#%F0%9F%87%AB%F0%9F%87%B7FR-13.37.22.159-9181
    trojan://892e4ff3-f8bb-42ac-9bd5-e103f235fc78@kr01.333210.xyz:40000?security=tls&sni=400567.xyz#%F0%9F%87%B0%F0%9F%87%B7KR-3.36.112.236-9063
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTphRnprSkppNE42SUxWU3NTVXpwb1A0@194.233.165.55:80#%F0%9F%87%A9%F0%9F%87%AADE-194.233.165.55-0800
    vmess://ewogICAgImFkZCI6ICJ2ZXJ5LnNhZG51Z2dldC5zaG9wIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmF5Lm51Z2dldHNlY3VyZS5idXp6IiwKICAgICJpZCI6ICJhNTMyNDUwMy0wNGJkLTRjZTQtYTQ3YS1lOTY5ZDYwNWE1YTYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbWFpbiIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzMuMjQ1LjU5LjE4MS0wMTg4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@195.154.169.198:989#%F0%9F%87%AB%F0%9F%87%B7FR-195.154.169.198-0785
    vmess://ewogICAgImFkZCI6ICI0My4yMDEuMjUzLjIyMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIjQzLjIwMS4yNTMuMjIyIiwKICAgICJpZCI6ICJjODQxYzkwMy03NjU3LTQxZjctYmY1NS1iNDFkZDk0NTYxNzkiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvYzg0MWM5MDMtNzY1Ny00MWY3LWJmNTUtYjQxZGQ5NDU2MTc5IiwKICAgICJwb3J0IjogMjY1NDAsCiAgICAicHMiOiAi8J+HsPCfh7dLUi00My4yMDEuMjUzLjIyMi0xOTExIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://842b5f9dd11e458d8613c907c4cc5723@202.64.1.167:443?security=tls&sni=www.gpt123.one#%F0%9F%87%AD%F0%9F%87%B0HK-202.64.1.167-0210
    trojan://telegram-id-directvpn@18.196.211.152:22222?security=tls&sni=trj.rollingnext.co.uk#%F0%9F%87%A9%F0%9F%87%AADE-18.196.211.152-0170
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpUMXBiN1h4eHJvbHZQU2IwdTJ4U09B@beacomf.xyz:8080#%F0%9F%87%A9%F0%9F%87%AADE-128.140.7.24-0787
    vmess://ewogICAgImFkZCI6ICI5NS4xNjQuODkuMjI1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI3MGE2OTRjOC1iYTY1LTRkMWQtOTQyZC00ZmM0ODlkYTFiNWYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMzgxNTMsCiAgICAicHMiOiAi8J+HqfCfh6pERS05NS4xNjQuODkuMjI1LTAyMDEiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1nY206am10Z3NtVzQwUg==@8.210.231.146:1146#%F0%9F%87%AD%F0%9F%87%B0HK-8.210.231.146-0517
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp1ZzRGdTc5U0VSRWRGR2x0MnNVeVQ0@95.164.9.144:2927#%F0%9F%87%A6%F0%9F%87%B9AT-95.164.9.144-9126
    ss://YWVzLTI1Ni1jZmI6cXdlclJFV1FAQA==@p222.panda001.net:54345#%F0%9F%87%B0%F0%9F%87%B7KR-125.141.31.71-0842
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@156.146.62.160:443#%F0%9F%87%A8%F0%9F%87%ADCH-156.146.62.160-0788
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@185.180.12.81:989#%F0%9F%87%A6%F0%9F%87%B9AT-185.180.12.81-0793
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3Ljc0IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJiOGE2YmY1OC00ODVhLTQwNDYtYjM4Ni1iMzY2MWJmNjVlZmYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvYmIiLAogICAgInBvcnQiOiAxMjM0NSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNzQtNDk2MCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMzAuMTYyLjQ3LjEyMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiYjVmN2U5MzItZjczMC00YWQyLWI0MjUtNDA5NzdiOWRiMzMyIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3pCTFBvdSIsCiAgICAicG9ydCI6IDY4NTQsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xMzAuMTYyLjQ3LjEyMy0xMTg4OSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpBSzRKMXNSdDJ2M2RMRFVWQzJQNWxq@94.131.12.245:37726#%F0%9F%87%A8%F0%9F%87%ADCH-94.131.12.245-7807
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpEcXVFSjZTSE92bk9YdGxzaUtEWXZr@3.74.55.245:443#%F0%9F%87%A9%F0%9F%87%AADE-3.74.55.245-0899
    vmess://ewogICAgImFkZCI6ICIxMzAuMTYyLjQ3LjEyMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiYjVmN2U5MzItZjczMC00YWQyLWI0MjUtNDA5NzdiOWRiMzMyIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3pCTFBvdSIsCiAgICAicG9ydCI6IDY4NTQsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xMzAuMTYyLjQ3LjEyMy0xMTg5MSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://842b5f9dd11e458d8613c907c4cc5723@149.28.151.140:443?security=tls&sni=www.gpt123.one#%F0%9F%87%B8%F0%9F%87%ACSG-149.28.151.140-0204
    ss://YWVzLTI1Ni1jZmI6ZjhucEtnTnpka3NzMnl0bg==@103.172.116.90:9088#%F0%9F%87%B8%F0%9F%87%ACSG-103.172.116.90-7889
    vmess://ewogICAgImFkZCI6ICIyMTcuMTYwLjQ1LjMxIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0ZTE4NjY3OC1mY2NhLTQzMjUtZTRiYy1iMjkxNmJkZjY3MDgiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogODg4MCwKICAgICJwcyI6ICLwn4ep8J+HqkRFLTIxNy4xNjAuNDUuMzEtMDQxNCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6S0JHalpZY3k0U3lSU2htQQ==@217.30.10.70:9044#%F0%9F%87%B5%F0%9F%87%B1PL-217.30.10.70-7793
    ss://YWVzLTI1Ni1jZmI6THAyN3JxeUpxNzJiWnNxWA==@103.172.116.90:9045#%F0%9F%87%B8%F0%9F%87%ACSG-103.172.116.90-9007
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@121.127.46.147:989#%F0%9F%87%B8%F0%9F%87%AASE-121.127.46.147-0813
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpYbFVGZ29PcURsVnFsWkZEM0pzMFlB@masting.xyz:8080#%F0%9F%87%B8%F0%9F%87%AASE-172.232.129.141-2440
    vmess://ewogICAgImFkZCI6ICIxMzkuNTkuMTIyLjIxMCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMDMzZmMwMTktZWQwMS00MzFmLTk2Y2UtNTI0MDg3ZTNlYzYyIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDgwODAsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0xMzkuNTkuMTIyLjIxMC0wMTY1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJmcjJlLXBvcnRtYXBwZXIudjJmcmVldnBuLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZyMmUtcG9ydG1hcHBlci52MmZyZWV2cG4uY29tIiwKICAgICJpZCI6ICIyYThhMTBmYi05Y2EzLTM2N2UtYTIzNC1jZjA5Zjg0MWJlNGYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZnJmcmZmZnZtbjAxTiIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMjEuNzEuODgtOTE2MiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpYbFVGZ29PcURsVnFsWkZEM0pzMFlB@masting.xyz:8080#%F0%9F%87%B8%F0%9F%87%AASE-172.232.129.141-0796
    ss://YWVzLTI1Ni1jZmI6NFIzaFVmWjJGSGhEbU5jUA==@103.172.116.79:9061#%F0%9F%87%B8%F0%9F%87%ACSG-103.172.116.79-0901
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@194.14.217.115:989#%F0%9F%87%B7%F0%9F%87%B4RO-194.14.217.115-0805
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpJVURuclhFeHBiMElWVkhzRXhzS1dM@51.21.126.136:443#%F0%9F%87%B8%F0%9F%87%AASE-51.21.126.136-0884
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@5.188.6.8:989#%F0%9F%87%BA%F0%9F%87%A6UA-5.188.6.8-0846
    vmess://ewogICAgImFkZCI6ICI0NS44Ny4xNTUuNzAiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjg4YzBhMWZiLWZjNGQtNGVhYi04NWM3LTRkZDg0NDA3ZTlhNSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi92bWVzcyIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh7rwn4emVUEtNDUuODcuMTU1LjcwLTkxMTEiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJmcjFlLXVubWV0ZXJlZC52MmZyZWV2cG4uY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiZnIxZS11bm1ldGVyZWQudjJmcmVldnBuLmNvbSIsCiAgICAiaWQiOiAiMmE4YTEwZmItOWNhMy0zNjdlLWEyMzQtY2YwOWY4NDFiZTRmIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3YxMzNQRFhra2x4TEVjT3ZEIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS43MS44OC0wMTc5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://842b5f9dd11e458d8613c907c4cc5723@185.151.146.211:443?security=tls&sni=www.gpt123.one#%F0%9F%87%B8%F0%9F%87%ACSG-185.151.146.211-0193
    ss://YWVzLTI1Ni1jZmI6S0JHalpZY3k0U3lSU2htQQ==@103.172.116.79:9044#%F0%9F%87%B8%F0%9F%87%ACSG-103.172.116.79-5506
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpFYUQyWFNKZ2tWTmpac3JycWVsUTFz@46.250.237.91:443#%F0%9F%87%AC%F0%9F%87%A7GB-46.250.237.91-0839
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@54.169.114.116:443#%F0%9F%87%B8%F0%9F%87%ACSG-54.169.114.116-9118
    trojan://842b5f9dd11e458d8613c907c4cc5723@38.180.105.115:443?security=tls&sni=www.gpt123.one#%F0%9F%87%B9%F0%9F%87%B7TR-38.180.105.115-0174
    ssr://NDUuODkuNTIuNjY6OTA0MTpvcmlnaW46YWVzLTI1Ni1jZmI6cGxhaW46VlRaeGJsbFNhR1o1UkcxdU9ITm5iZz09Lz9vYmZzcGFyYW09JnJlbWFya3M9OEolMkJIdWZDZmg3ZFVVaTAwTlM0NE9TNDFNaTQyTmkwNU1EUTQmcHJvdG9wYXJhbT0=
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@185.164.35.9:989#%F0%9F%87%A7%F0%9F%87%A6BA-185.164.35.9-0859
    ss://YWVzLTI1Ni1jZmI6UzdLd1V1N3lCeTU4UzNHYQ==@45.89.52.66:9042#%F0%9F%87%B9%F0%9F%87%B7TR-45.89.52.66-0872
    ss://YWVzLTI1Ni1jZmI6VTZxbllSaGZ5RG1uOHNnbg==@45.89.52.66:9041#%F0%9F%87%B9%F0%9F%87%B7TR-45.89.52.66-0876
    vmess://ewogICAgImFkZCI6ICIxNzIuNjcuMjM1LjIzNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInd3dy4zMTAwMG9vb293ZTIuYmYiLAogICAgImlkIjogImYyNGJiYTBmLTg2NTYtNDRmOC1iMjFlLWEwZTNhMTkwYzRjNSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kZjk3YjIxZS0zOTQzLTQ4NjUtYWYxOC1iNWVhOTY3NmIwMzciLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42Ny4yMzUuMjM3LTE4MjEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJiczEubG9hZGluZ2lwLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImJzMS5sb2FkaW5naXAuY29tIiwKICAgICJpZCI6ICI5ZTU5OTliYS04NzBhLTQ2YjEtODUwMC0zN2M2NDAzNzFlYzYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvYnMiLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4e78J+Hs1ZOLTEwMy4yNTIuOTQuMjAyLTE3MzkiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJmcmVlLm1hbmc1Zy5tZSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZyZWUubWFuZzVnLm1lIiwKICAgICJpZCI6ICI4YTJhN2I5Mi1iNjVkLTQxNTUtOTFmYy03YjdiZTUyY2E1OTgiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbWFuZzVnLm1lIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+Hu/Cfh7NWTi0xMDMuNzUuMTg1LjEzMC0xOTIyIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6cXdlclJFV1FAQA==@p234.panda004.net:56906#%F0%9F%87%B0%F0%9F%87%B7KR-222.112.15.140-0834
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@34.222.2.189:443#%F0%9F%87%BA%F0%9F%87%B8US-34.222.2.189-9136
    vmess://ewogICAgImFkZCI6ICIxNzYuMTIwLjc0LjE0MiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImludGVybmV0LmxpZmUuY29tLmJ5IiwKICAgICJpZCI6ICI3NTY5NWY1YS1iNmFmLTQ0ZjQtOTk4My1hZTI1MGI1M2ZmOWMiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh6rwn4e4RVMtMTc2LjEyMC43NC4xNDItMDgzNiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpkYXRkR0ZlNExrTU43MTBhSGVkeQ==@85.239.52.174:51348#%F0%9F%87%BA%F0%9F%87%B8US-85.239.52.174-0869
    ss://YWVzLTI1Ni1nY206d3dxNlhvNWdKOA==@38.54.104.184:18808#%F0%9F%87%BA%F0%9F%87%B8US-38.54.104.184-0530
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@180.149.44.120:989#%F0%9F%87%A6%F0%9F%87%BFAZ-180.149.44.120-0847
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:803#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-0844
    vmess://ewogICAgImFkZCI6ICI4MC45Mi4yMDUuMTEyIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiODAuOTIuMjA1LjExMiIsCiAgICAiaWQiOiAiNGM5MGJhNzUtMjMwYi00ZjhiLWJiZmYtOGVmYTBlYjA0MTVmIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTgwLjkyLjIwNS4xMTItMDgwNiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:811#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-0868
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:804#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-0857
    ssr://NDMuMjAxLjE0Ny4xNTE6NDQzOm9yaWdpbjphZXMtMjU2LWNmYjpwbGFpbjpZVzFoZW05dWMydHlNRFU9Lz9vYmZzcGFyYW09JnJlbWFya3M9OEolMkJIc1BDZmg3ZExVaTAwTXk0eU1ERXVNVFEzTGpFMU1TMDVNRFF5JnByb3RvcGFyYW09
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:806#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-0861
    vmess://ewogICAgImFkZCI6ICJza3lodDIudnBuZGF0YS52biIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNreWh0Mi52cG5kYXRhLnZuIiwKICAgICJpZCI6ICJmYmNjZmVkNy0xYWViLTQxNmEtYTRmZC03YWYxNzQ3ZjlmM2IiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvVlBOREFUQS5WUE4iLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4e78J+Hs1ZOLTExNS43OS4yMzguMzQtOTE5NiIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogZmFsc2UsCiAgICAic25pIjogImxpZW5xdWFuLmdhcmVuYS52biIKfQ==
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@74.121.191.98:989#%F0%9F%87%BA%F0%9F%87%B8US-74.121.191.98-11198
    vmess://ewogICAgImFkZCI6ICJjZmNkbjIuc2FuZmVuY2RuOS5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICI3bkFpNzRqSnNnMS55b2ZuaGtmYy54eXoiLAogICAgImlkIjogImQwYTNlMDhhLWQyNmYtNDViZC1iYTNjLTYzODdmOTE4MjYzMyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi92aWRlby9jOWVmeFJDaSIsCiAgICAicG9ydCI6IDIwNTIsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNzQuMTk0LTAyMDIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://f63c1106-be09-4479-b214-aef555f9fc44@13.49.127.111:443?security=tls&sni=north-1.compute.seatech.ir#%F0%9F%87%B8%F0%9F%87%AASE-13.49.127.111-3724
    vmess://ewogICAgImFkZCI6ICIxNzMuMjQ1LjU4LjY1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmF5Lm51Z2dldHNlY3VyZS5idXp6IiwKICAgICJpZCI6ICJhNTMyNDUwMy0wNGJkLTRjZTQtYTQ3YS1lOTY5ZDYwNWE1YTYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbWFpbiIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzMuMjQ1LjU4LjY1LTE4OTMiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ssr://MTAzLjE3Mi4xMTYuNzk6OTAyMDpvcmlnaW46YWVzLTI1Ni1jZmI6cGxhaW46UWs1dFFWaFllRUZJV1hCVVVtUjZkUT09Lz9vYmZzcGFyYW09JnJlbWFya3M9OEolMkJIdVBDZmg2eFRSeTB4TURNdU1UY3lMakV4Tmk0M09TMDVNalE0JnByb3RvcGFyYW09
    vmess://ewogICAgImFkZCI6ICIxODIuMTYuMS4xOTQiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjAwYTFkYTE0LWQ1NWYtNWY3NS1lMzQ2LTc5Yjk4NWUxYTcyMyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9vcHQvdmlkZW8vaW1hZ2VzIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+HrfCfh7BISy0xODIuMTYuMS4xOTQtOTA4NCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@213.169.137.221:989#%F0%9F%87%A8%F0%9F%87%BECY-213.169.137.221-0866
    ss://YWVzLTI1Ni1jZmI6QndjQVVaazhoVUZBa0RHTg==@45.89.52.66:9031#%F0%9F%87%B9%F0%9F%87%B7TR-45.89.52.66-0903
    vmess://ewogICAgImFkZCI6ICI0My4yMDEuMjUzLjIyMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiYzg0MWM5MDMtNzY1Ny00MWY3LWJmNTUtYjQxZGQ5NDU2MTc5IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2M4NDFjOTAzLTc2NTctNDFmNy1iZjU1LWI0MWRkOTQ1NjE3OSIsCiAgICAicG9ydCI6IDI2NTQwLAogICAgInBzIjogIvCfh7Dwn4e3S1ItNDMuMjAxLjI1My4yMjItNzY5NyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogZmFsc2UsCiAgICAic25pIjogIjQzLjIwMS4yNTMuMjIyIgp9
    vmess://ewogICAgImFkZCI6ICJjZmNkbjMuc2FuZmVuY2RuOS5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJhZ3pianN6dWpwNC55b2ZuaGtmYy54eXoiLAogICAgImlkIjogImQwYTNlMDhhLWQyNmYtNDViZC1iYTNjLTYzODdmOTE4MjYzMyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi92aWRlby9pYkNUNno1NSIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTkuMjQ1LjE1NC0wMTk1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp0dlgxdiNOU0ZQX0xHX2JK@169.197.141.186:801#%F0%9F%87%BA%F0%9F%87%B8US-169.197.141.186-0849
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@103.163.218.2:989#%F0%9F%87%BB%F0%9F%87%B3VN-103.163.218.2-0851
    ss://YWVzLTI1Ni1jZmI6VE4yWXFnaHhlRkRLWmZMVQ==@5.188.181.201:9037#%F0%9F%87%AA%F0%9F%87%B8ES-5.188.181.201-0856
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@62.12.116.66:989#%F0%9F%87%B0%F0%9F%87%AAKE-62.12.116.66-0853
    ss://YWVzLTI1Ni1jZmI6VE4yWXFnaHhlRkRLWmZMVQ==@45.89.52.66:9037#%F0%9F%87%B9%F0%9F%87%B7TR-45.89.52.66-11291
    ss://YWVzLTI1Ni1jZmI6cDl6NUJWQURIMllGczNNTg==@45.89.52.66:9040#%F0%9F%87%B9%F0%9F%87%B7TR-45.89.52.66-11290
    ss://YWVzLTI1Ni1jZmI6cDl6NUJWQURIMllGczNNTg==@5.188.181.201:9040#%F0%9F%87%AA%F0%9F%87%B8ES-5.188.181.201-0873
    vmess://ewogICAgImFkZCI6ICIxNTguMTAxLjcuOCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiOTViNDVjNDktZjVjMC00OTU5LWJiNjQtMmI4ZmJjNGE4NjljIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh7rwn4e4VVMtMTU4LjEwMS43LjgtMTE3NDMiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1jZmI6R2VyZWdldFI4Y3ZRSHpZcg==@5.188.181.201:9030#%F0%9F%87%AA%F0%9F%87%B8ES-5.188.181.201-0877
    ssr://MjE3LjMwLjEwLjY4OjkwNzk6b3JpZ2luOmFlcy0yNTYtY2ZiOnBsYWluOlZGQnhXRGhsWkdkaVFWVlNZMEZOWWc9PS8/b2Jmc3BhcmFtPSZyZW1hcmtzPThKJTJCSHRmQ2ZoN0ZRVEMweU1UY3VNekF1TVRBdU5qZ3RPVEEwTkElM0QlM0QmcHJvdG9wYXJhbT0=
    ss://YWVzLTI1Ni1jZmI6Z1lDWVhma1VRRXMyVGFKUQ==@217.30.10.68:9038#%F0%9F%87%B5%F0%9F%87%B1PL-217.30.10.68-0900
    ssr://NS4xODguMTgxLjIwMTo5MDMwOm9yaWdpbjphZXMtMjU2LWNmYjpwbGFpbjpSMlZ5WldkbGRGSTRZM1pSU0hwWmNnPT0vP29iZnNwYXJhbT0mcmVtYXJrcz04SiUyQkhxdkNmaDdoRlV5MDFMakU0T0M0eE9ERXVNakF4TFRrd05EVSUzRCZwcm90b3BhcmFtPQ==
    vmess://ewogICAgImFkZCI6ICIxMjkuMTUxLjE2NC4xNTIiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogImUzMGY4NTg4LTI1NTUtNDhiOC1jMzU0LWM4ZTYzZjU3MjMyZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiA1NTYwMCwKICAgICJwcyI6ICLwn4e/8J+HplpBLTEyOS4xNTEuMTY0LjE1Mi0wMTY0IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@3.113.1.121:443#%F0%9F%87%AF%F0%9F%87%B5JP-3.113.1.121-9002
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@190.103.176.29:989#%F0%9F%87%A6%F0%9F%87%B7AR-190.103.176.29-0874
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@185.90.61.153:989#%F0%9F%87%B3%F0%9F%87%B4NO-185.90.61.153-0864
    vmess://ewogICAgImFkZCI6ICI5NC4xMzEuMTE3LjE1OSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiNzJiM2I4OWEtMzBjNS00ZGM3LThiNmUtZjYxMjE4Yjk1ZWRhIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3ZtZXNzIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+HqvCfh7hFUy05NC4xMzEuMTE3LjE1OS0wMTU4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJocmdkdnBuLmZseWNkbmVkYzU1LnZpcCIsCiAgICAiYWlkIjogMzIsCiAgICAiaG9zdCI6ICJocmdkdnBuLmZseWNkbmVkYzU1LnZpcCIsCiAgICAiaWQiOiAiMDBhMWRhMTQtZDU1Zi01Zjc1LWUzNDYtNzliOTg1ZTFhNzIzIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL29wdC92aWRlby9pbWFnZXMiLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4et8J+HsEhLLTE4Mi4xNi4xLjE5NC0xMTA3MSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ssr://cDE0MS5wYW5kYTAwMS5uZXQ6NTQzNDU6b3JpZ2luOmFlcy0yNTYtY2ZiOnBsYWluOmNYZGxjbEpGVjFGQVFBPT0vP29iZnNwYXJhbT0mcmVtYXJrcz04SiUyQkhzUENmaDdkTFVpMHlNVGd1TWpNM0xqRTROUzR5TXpBdE9UQTBOZyUzRCUzRCZwcm90b3BhcmFtPQ==
    vmess://ewogICAgImFkZCI6ICI3Ny43NS4yMzAuMTI1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJkNDY2ZGQzNi04Yjg2LTQ4YjctYjBmMC02N2U3ZDEyOGRlNmMiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvdm1lc3MiLAogICAgInBvcnQiOiAyMDgyLAogICAgInBzIjogIvCfh6jwn4e/Q1otNzcuNzUuMjMwLjEyNS05MDcyIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ssr://MTAzLjE3Mi4xMTYuOTA6OTAzMTpvcmlnaW46YWVzLTI1Ni1jZmI6cGxhaW46UW5kalFWVmFhemhvVlVaQmEwUkhUZz09Lz9vYmZzcGFyYW09VG05dVpRJTNEJTNEJnJlbWFya3M9OEolMkJIdVBDZmg2eFRSeTB4TURNdU1UY3lMakV4Tmk0NU1DMDVNakl6JnByb3RvcGFyYW09
    trojan://telegram-id-privatevpns@99.81.90.199:22222?security=tls&sni=trojan.miwan.co.uk#%F0%9F%87%AE%F0%9F%87%AAIE-99.81.90.199-2101
    trojan://f63c1106-be09-4479-b214-aef555f9fc44@ec2-13-49-127-111.eu-north-1.compute.amazonaws.com:443?security=tls&sni=north-1.compute.seatech.ir#%F0%9F%87%B8%F0%9F%87%AASE-13.49.127.111-9116
    ssr://MTAzLjE3Mi4xMTYuOTA6OTA0MTpvcmlnaW46YWVzLTI1Ni1jZmI6cGxhaW46VlRaeGJsbFNhR1o1UkcxdU9ITm5iZz09Lz9vYmZzcGFyYW09VG05dVpRJTNEJTNEJnJlbWFya3M9OEolMkJIdVBDZmg2eFRSeTB4TURNdU1UY3lMakV4Tmk0NU1DMDVNakl5JnByb3RvcGFyYW09
    ss://YWVzLTI1Ni1jZmI6ZGFGWWFncURkQmRBNlZUWA==@217.30.10.68:9073#%F0%9F%87%B5%F0%9F%87%B1PL-217.30.10.68-0911
    vmess://ewogICAgImFkZCI6ICJtaW5nMi5raXdpcmVpY2guY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibWluZzIua2l3aXJlaWNoLmNvbSIsCiAgICAiaWQiOiAiMThlNWY0MGYtYmRhNi00YzE1LTkzMzQtZTg3Y2RhNjA0N2FmIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3JheSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjIxLjEyLjEwMy0yMzY0IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6VVRKQTU3eXBrMlhLUXBubQ==@217.30.10.68:9033#%F0%9F%87%B5%F0%9F%87%B1PL-217.30.10.68-7784
    vmess://ewogICAgImFkZCI6ICJzazEtdm1lc3Muc3NobWF4Lnh5eiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNrMS12bWVzcy5zc2htYXgueHl6IiwKICAgICJpZCI6ICIwNmMyYjU2OC1iN2RmLTRlODAtOTAzMS1jODM1NjkzOTdkYjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvdm1lc3MiLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4e48J+HsFNLLTUuMjUyLjIzLjEzMy05MTEyIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@190.120.230.9:989#%F0%9F%87%A8%F0%9F%87%B1CL-190.120.230.9-0870
    vmess://ewogICAgImFkZCI6ICIxMDQuMTguMjAyLjIzMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNhNC50ZWhtZTIuZnVuIiwKICAgICJpZCI6ICI1OGZlMTU0Mi01MjkwLTQwYWQtODE1YS03NzcwN2E4MWFmZTUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvSU9lYmhMTWhsMUNUYkZIYkw5NW15ZlJYMiIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfj4FSRUxBWS0xMDQuMTguMjAyLjIzMi0xMzc5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6YW1hem9uc2tyMDU=@43.203.119.237:443#%F0%9F%87%B0%F0%9F%87%B7KR-43.203.119.237-5331
    ss://YWVzLTI1Ni1jZmI6cXdlclJFV1FAQA==@p141.panda001.net:54345#%F0%9F%87%B0%F0%9F%87%B7KR-218.237.185.230-7771
    vmess://ewogICAgImFkZCI6ICIxMDQuMzEuMTYuMjgiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJjYTQudGVobWUyLmZ1biIsCiAgICAiaWQiOiAiNThmZTE1NDItNTI5MC00MGFkLTgxNWEtNzc3MDdhODFhZmU1IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL0lPZWJoTE1obDFDVGJGSGJMOTVteWZSWDIiLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjMxLjE2LjI4LTQxNjQiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1jZmI6RkFkVXZNSlVxNXZEZ0tFcQ==@217.30.10.68:9006#%F0%9F%87%B5%F0%9F%87%B1PL-217.30.10.68-11438
    ss://YWVzLTI1Ni1jZmI6Z1lDWVhma1VRRXMyVGFKUQ==@103.172.116.79:9038#%F0%9F%87%B8%F0%9F%87%ACSG-103.172.116.79-9206
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.172.113.182:811#%F0%9F%87%AF%F0%9F%87%B5JP-185.172.113.182-0893
    vmess://ewogICAgImFkZCI6ICI5NC4xMzEuOTcuMTIzIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiY3oxLXZtZXNzLnNzaG1heC54eXoiLAogICAgImlkIjogImQ0NjZkZDM2LThiODYtNDhiNy1iMGYwLTY3ZTdkMTI4ZGU2YyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi92bWVzcyIsCiAgICAicG9ydCI6IDIwODIsCiAgICAicHMiOiAi8J+HqPCfh79DWi05NC4xMzEuOTcuMTIzLTUzODkiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxODguMTE0Ljk4LjIxOSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImRvbmF0ZS5zaGFkb3dicm93c2Uub25saW5lIiwKICAgICJpZCI6ICJkMWNiYWQ4MS1hMmExLTQ0MTktODg0MC1mNmNlMDlkNGY4NjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbWFpbiIsCiAgICAicG9ydCI6IDIwODYsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE4OC4xMTQuOTguMjE5LTAyMDUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@190.120.231.45:989#%F0%9F%87%A8%F0%9F%87%B4CO-190.120.231.45-0885
    vmess://ewogICAgImFkZCI6ICJocmdkdnBuLmZseWNkbmVkYzU1LnZpcCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICJocmdkdnBuLmZseWNkbmVkYzU1LnZpcCIsCiAgICAiaWQiOiAiMDBhMWRhMTQtZDU1Zi01Zjc1LWUzNDYtNzliOTg1ZTFhNzIzIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL29wdC92aWRlby9pbWFnZXMiLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4et8J+HsEhLLTE4Mi4xNi4xLjE5NC0xMTA2OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJjejEtdm1lc3Muc3NobWF4Lnh5eiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImN6MS12bWVzcy5zc2htYXgueHl6IiwKICAgICJpZCI6ICJkNDY2ZGQzNi04Yjg2LTQ4YjctYjBmMC02N2U3ZDEyOGRlNmMiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvdm1lc3MiLAogICAgInBvcnQiOiAyMDgyLAogICAgInBzIjogIvCfh6jwn4e/Q1otOTQuMTMxLjk3LjEyMy01MzI2IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiBmYWxzZSwKICAgICJzbmkiOiAiY3oxLXZtZXNzLnNzaG1heC54eXoiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpRNUNFaWViU3VTbDJxRmtmRTR6dEcy@45.8.147.80:5741#%F0%9F%87%B8%F0%9F%87%AASE-45.8.147.80-0906

    vmess://ewogICAgImFkZCI6ICJ3d3cuZ292LmhrIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibGludXMuY2xvdWRmbGFyZS5xdWVzdCIsCiAgICAiaWQiOiAiMWFiOTFmMTgtNjE2OC00Y2I2LWM5Y2EtMmMzYzcxNThmZTRjIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2FyaWVzIiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE2LjI0OS4xMzAtMTMwMSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTEyOC1jZmI6c2hhZG93c29ja3M=@156.146.38.163:443#%F0%9F%87%BA%F0%9F%87%B8US-156.146.38.163-0799
    vmess://ewogICAgImFkZCI6ICJ4ci0xLmhlcm9rdWFwcC5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ4ci0xLmhlcm9rdWFwcC5jb20iLAogICAgImlkIjogIjE3YWY3NmUxLWE1ZDctNDFhYi1hZTg3LWI0OGYxODUwNzVkMSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8xN2FmNzZlMS1hNWQ3LTQxYWItYWU4Ny1iNDhmMTg1MDc1ZDEtdm1lc3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy01NC4yNDMuMTI5LjIxNS0xOTA1MCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@172.96.192.58:254#%F0%9F%87%BA%F0%9F%87%B8US-172.96.192.58-0463
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@97.64.31.80:247#%F0%9F%87%BA%F0%9F%87%B8US-97.64.31.80-0461
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@144.168.60.70:252#%F0%9F%87%BA%F0%9F%87%B8US-144.168.60.70-15607
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNC4yMCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMS50cnVtcDIwMjMubmV0IiwKICAgICJpZCI6ICIxNzZiNTk4Zi00NDViLTQxYWMtOWQyYS00MzBjNWM0ZGYyNmEiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNDEuMTAxLjExNC4yMC0wMjk0IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@172.96.192.100:246#%F0%9F%87%BA%F0%9F%87%B8US-172.96.192.100-15615
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICJ3d3cuMTcwODAxMDAueHl6IiwKICAgICJpZCI6ICIyNTY2ZDAwZi0yMThjLTQ4ZjctOWEzNi0xM2QzZDZmMWE3MjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xNzM0MTgxNDExMjMiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy02Ny4yMS43Mi40MS01NTE4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDY=@95.169.4.174:254#%F0%9F%87%BA%F0%9F%87%B8US-95.169.4.174-15616
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDM=@104.243.25.95:253#%F0%9F%87%BA%F0%9F%87%B8US-104.243.25.95-0436
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@144.168.58.170:254#%F0%9F%87%BA%F0%9F%87%B8US-144.168.58.170-15618
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@107.182.177.136:256#%F0%9F%87%BA%F0%9F%87%B8US-107.182.177.136-0659
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDY=@93.179.112.70:253#%F0%9F%87%BA%F0%9F%87%B8US-93.179.112.70-15619
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiaWQiOiAiMjU2NmQwMGYtMjE4Yy00OGY3LTlhMzYtMTNkM2Q2ZjFhNzI0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3BhdGgvMTczNDE4MTQxMTIzIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtNjcuMjEuNzIuNDEtOTg3OCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@97.64.122.63:253#%F0%9F%87%BA%F0%9F%87%B8US-97.64.122.63-15606
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40MSIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjI1NjZkMDBmLTIxOGMtNDhmNy05YTM2LTEzZDNkNmYxYTcyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzE3MzQxODE0MTEyMyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTY3LjIxLjcyLjQxLTQ4OTQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJ2dXMyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVzMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy00NS4zMy4xMDUuMjM5LTEwODE3IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJ2dXMzLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVzMy4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy00NS43OS4yMjQuNTMtMTExNyIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICJ3d3cuNDg4MTY2MjYueHl6IiwKICAgICJpZCI6ICIyNTY2ZDAwZi0yMThjLTQ4ZjctOWEzNi0xM2QzZDZmMWE3MjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMDgzMDE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HuvCfh7hVUy02Ny4yMS43Mi40NC00ODkxIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDU=@198.181.56.163:238#%F0%9F%87%BA%F0%9F%87%B8US-198.181.56.163-15629
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjI1NjZkMDBmLTIxOGMtNDhmNy05YTM2LTEzZDNkNmYxYTcyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzEyMDIwODMwMTQyMiIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTY3LjIxLjcyLjQ0LTEwMzA5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICI2Ny4yMS43Mi40NCIsCiAgICAiaWQiOiAiMjU2NmQwMGYtMjE4Yy00OGY3LTlhMzYtMTNkM2Q2ZjFhNzI0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL3BhdGgvMTIwMjA4MzAxNDIyIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7rwn4e4VVMtNjcuMjEuNzIuNDQtMTAyODEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.198:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.198-0803
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.79:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.79-0800
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.193:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.193-0998
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.81:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.81-0561
    trojan://e23f408a-012e-4030-8b31-02022031cb50@fhcamd1.gaox.ml:443?allowInsecure=1#%F0%9F%87%BA%F0%9F%87%B8US-129.146.135.157-16738
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.194:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.194-0535
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.195:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.195-0802
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.78:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.78-0533
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.196:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.196-1355
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.80:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.80-0997
    ss://YWVzLTEyOC1nY206c2hhZG93c29ja3M=@212.102.53.197:443#%F0%9F%87%AC%F0%9F%87%A7GB-212.102.53.197-0562
    vmess://ewogICAgImFkZCI6ICIxMjkuMTU5LjQxLjIzMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMzQxYTkxODItYzQyMy00OTljLWM0NmUtZDE3ODM4YjI5MDM3IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDMyNTg2LAogICAgInBzIjogIvCfh7rwn4e4VVMtMTI5LjE1OS40MS4yMzMtMDIzOSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMjkuMTQ2LjEzMy4xNTciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjgxNzE0Y2VmLTliZGUtNGEwOC1hYTUwLWQ2YmMwMTcyZDc4YiIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiA1MTAwOSwKICAgICJwcyI6ICLwn4e68J+HuFVTLTEyOS4xNDYuMTMzLjE1Ny0wMjc1IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTU0LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoNi5zc3ItZnJlZS54eXoiLAogICAgImlkIjogIjVmNjRmYTY1LTdiMTQtNDljNS05NTRkLWFhMTVjNmJmY2FjZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTQuMTUwLTAyNTEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@78.129.253.9:808#%F0%9F%87%AC%F0%9F%87%A7GB-78.129.253.9-15647
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@78.129.253.9:809#%F0%9F%87%AC%F0%9F%87%A7GB-78.129.253.9-1394
    ss://YWVzLTI1Ni1jZmI6Yndoc2tyc2tyMDE=@65.49.204.125:254#%F0%9F%87%BA%F0%9F%87%B8US-65.49.204.125-15627
    vmess://ewogICAgImFkZCI6ICJ2dWsyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidnVrMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi0xMDkuNzQuMTk0LjIwOC0xMjQ5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:808#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15739
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTU1LjIwMSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMy50cnVtcDIwMjMub3JnIiwKICAgICJpZCI6ICIyOGRhZDY5Yy1jOWQ2LTQ3YzUtYWQwNS1jNjZhZmI4N2NjYmQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xNzIuNjQuMTU1LjIwMS0wMjY2IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxOTguNDEuMjEyLjEwMCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZyMS5jZmNkbjEueHl6IiwKICAgICJpZCI6ICJmYjViYmM4Yy1mNmVjLTQ2MjktOGM5ZS0yM2YwMjc4MWEyMGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZG9uZ3RhaXdhbmcuY29tIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfj4FSRUxBWS0xOTguNDEuMjEyLjEwMC04NjEwIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:800#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15732
    vmess://ewogICAgImFkZCI6ICJ2ZGUxLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmRlMS4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xNzIuMTA1LjI0NS43OS0wMjk4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJ2ZGUyLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidmRlMi4wYmFkLmNvbSIsCiAgICAiaWQiOiAiOTI3MDk0ZDMtZDY3OC00NzYzLTg1OTEtZTI0MGQwYmNhZTg3IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2NoYXQiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HqfCfh6pERS0xMzkuMTQ0LjE3Ni43Ni0xMjgwIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.178:804#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.178-14790
    vmess://ewogICAgImFkZCI6ICJzdHJlYW0uYXphZHJhaDIyLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInN0cmVhbS5hemFkcmFoMjIuY29tIiwKICAgICJpZCI6ICI3NmUxNTFhNy05OTgwLTQwNzctYmQ1Mi0wN2VmNGU5Y2I0OTYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvdXNlciIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh67wn4e3SVItMTg1LjE0My4yMzQuMTIwLTE5NDk5IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:805#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15756
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:806#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15744
    vmess://ewogICAgImFkZCI6ICJzdHVkeW5ldy5jbiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInN0dWR5bmV3LmNuIiwKICAgICJpZCI6ICJiYjg0NzI1YS1mNzI2LTRiY2ItODEzMS00NGRmMTIwOTQwMDUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvZGVuZ3FpbmdibyIsCiAgICAicG9ydCI6IDUxMzQwLAogICAgInBzIjogIvCfh7rwn4e4VVMtMTk4LjE0OC4xMjcuNjItOTgxOSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI4NS4xNy41LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIjg1LjE3LjUuMTUwIiwKICAgICJpZCI6ICI0MDcwZmRkZS00M2Q1LTRiM2YtZGJjZi03NzUxYzc3ZTRiZjYiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvQWY1NjQ1dHIiLAogICAgInBvcnQiOiAzNjMwNiwKICAgICJwcyI6ICLwn4ez8J+HsU5MLTg1LjE3LjUuMTUwLTExNjE4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICI4NS4xNy41LjE1MCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiNDA3MGZkZGUtNDNkNS00YjNmLWRiY2YtNzc1MWM3N2U0YmY2IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL0FmNTY0NXRyIiwKICAgICJwb3J0IjogMzYzMDYsCiAgICAicHMiOiAi8J+Hs/Cfh7FOTC04NS4xNy41LjE1MC0xMTYxMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:801#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15782
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:807#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0966
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:811#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-2149
    ss://YWVzLTI1Ni1jZmI6ZjhmN2FDemNQS2JzRjhwMw==@194.71.126.31:989#%F0%9F%87%B7%F0%9F%87%B8RS-194.71.126.31-0408
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNS4xMjAiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJsZzEuY2ZjZG4zLnh5eiIsCiAgICAiaWQiOiAiMzNhYTU3ZGYtMWM5My00MzE4LTlmY2UtZTg1MDQzN2VlNzgxIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2Rvbmd0YWl3YW5nLmNvbSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4+BUkVMQVktMTQxLjEwMS4xMTUuMTIwLTEyMzQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://8b6daf15-8342-482d-b894-1239fd98ce7f@149.56.141.11:443?allowInsecure=1#%F0%9F%87%A8%F0%9F%87%A6CA-149.56.141.11-0319
    ssr://NDUuMTU0LjIxNS4xMzU6MzE1ODA6YXV0aF9hZXMxMjhfc2hhMTphZXMtMjU2LWNmYjp0bHMxLjJfdGlja2V0X2F1dGg6ZW5oUGJXUkUvP29iZnNwYXJhbT1WbTB4TkdFd01VaFNXR2hVVjBkNFYxbHJaRk5XYkd4VlUycFNXRkp0ZUhwWGEyTTFZV3hLZEdWSWNGaGhNVlV4VmtkNFlXTXhXbkZXYkZaWFlsZG9VVmRXVm1GVGJWRjVWR3RXVW1KSGFGbFZha0YzJnJlbWFya3M9OEolMkJIdXZDZmg3aFZVeTAwTlM0eE5UUXVNakUxTGpFek5TMHlNemcxJnByb3RvcGFyYW09TWpJMk5qTTZVWEZNYjJGWg==
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMTY5ODkiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://8b6daf15-8342-482d-b894-1239fd98ce7f@cat1.sshocean.net:443?allowInsecure=1#%F0%9F%87%A8%F0%9F%87%A6CA-149.56.141.11-0241
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTo5N09uREVaWUdqYTQ=@178.18.244.2:443#%F0%9F%87%A9%F0%9F%87%AADE-178.18.244.2-0756
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpzaUY5OHhCTDJ2MWk=@135.181.114.242:8478#%F0%9F%87%AB%F0%9F%87%AEFI-135.181.114.242-0798
    ss://YWVzLTI1Ni1jZmI6R2VyZWdldFI4Y3ZRSHpZcg==@213.183.53.221:9030#%F0%9F%87%B7%F0%9F%87%BARU-213.183.53.221-15695
    ss://YWVzLTI1Ni1jZmI6ZjhucEtnTnpka3NzMnl0bg==@213.183.53.221:9088#%F0%9F%87%B7%F0%9F%87%BARU-213.183.53.221-15694
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTopMU4xRTZ2MFNVX3JHVHBn@38.64.138.53:1035#%F0%9F%87%BA%F0%9F%87%B8US-38.64.138.53-0573
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.47:805#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.47-0761
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.161.118.38:812#%F0%9F%87%A8%F0%9F%87%A6CA-51.161.118.38-15779
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpXYWN3ZXRDaWY=@217.12.223.190:444#%F0%9F%87%BA%F0%9F%87%A6UA-217.12.223.190-0790
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:808#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-13651
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@5.188.0.151:800#%F0%9F%87%BA%F0%9F%87%B8US-5.188.0.151-15704
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@ak1466.free.www.outline.network:811#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-7643
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:809#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0566
    ssr://anAtYW00OC02LmVxbm9kZS5uZXQ6ODA4MTpvcmlnaW46YWVzLTI1Ni1jZmI6dGxzMS4yX3RpY2tldF9hdXRoOlpVRnZhMkpoUkU0Mi8/b2Jmc3BhcmFtPSZyZW1hcmtzPThKJTJCSHIlMkZDZmg3VktVQzAxTkM0Mk5DNDFOeTR6TkMwd05UYzQmcHJvdG9wYXJhbT0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:805#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15687
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiNTEuODkuNDIuMTU0IiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMTEzNTciLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNDEuMTAxLjExNS4yIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiZnIxLmNmY2RuMS54eXoiLAogICAgImlkIjogImZiNWJiYzhjLWY2ZWMtNDYyOS04YzllLTIzZjAyNzgxYTIwZCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE0MS4xMDEuMTE1LjItMDI0NCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNTAuMjMwLjE5OS4xNzciLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjZiNzQ1Y2FmLWU3ZjYtNDlmMS05YjYzLWU1YzQxNjMwM2JhYyIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAyMTY5NiwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1MC4yMzAuMTk5LjE3Ny0wMjM3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNDQuMjQuODguMTAxIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJmNTQyNWNjZi0zOTQ2LTRmYjQtZWIyNC01MzkzZDc4YTM5MmYiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTY4MzMsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNDQuMjQuODguMTAxLTA0NzYiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.143:802#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.143-15751
    vmess://ewogICAgImFkZCI6ICIxMzguMi4xNS4yMyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiOTk4MTUxZTUtMGJjNS00Mzc3LWUzOTAtYzQxYmIyNmZkZDBjIiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDQ2MzcwLAogICAgInBzIjogIvCfh6/wn4e1SlAtMTM4LjIuMTUuMjMtMDI5MCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJ2bTEyLmxlaWZlbmdrZWppLmxpdmUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ2bTEyLmxlaWZlbmdrZWppLmxpdmUiLAogICAgImlkIjogIjc1MmE5NDA0LWM3MjktNDg1ZS04ZWE1LWFjYjNmNGZjODE4MCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAxMTExMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTQzLjIwMS4zOC4xOTMtMTI5OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJ2bTUubGVpZmVuZ2tlamkubGl2ZSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInZtNS5sZWlmZW5na2VqaS5saXZlIiwKICAgICJpZCI6ICI3NTJhOTQwNC1jNzI5LTQ4NWUtOGVhNS1hY2IzZjRmYzgxODAiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMTExMTEsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xMy4yMDkuNC4yMTEtMDIyOCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://752a9404-c729-485e-8ea5-acb3f4fc8180@hg5.leifengkeji.live:48903?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-43.200.4.201-11721
    vmess://ewogICAgImFkZCI6ICIxNTIuNzAuMjQxLjE4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJlY2QyNzRjMC0xNzVkLTQ1ZjctODI3Ni1hM2RhOTM3ODY2MzIiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMjY2NzYsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNTIuNzAuMjQxLjE4LTAzMjgiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxOTIuNzQuMjQyLjE4MiIsCiAgICAiYWlkIjogNjQsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjQxODA0OGFmLWEyOTMtNGI5OS05YjBjLTk4Y2EzNTgwZGQyNCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9wYXRoLzE3MDQxOTExMTAyMSIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e68J+HuFVTLTE5Mi43NC4yNDIuMTgyLTE2NjgzIiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICJ3d3cuMzIzMzgwNzUueHl6Igp9
    vmess://ewogICAgImFkZCI6ICJ2bTgubGVpZmVuZ2tlamkubGl2ZSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInZtOC5sZWlmZW5na2VqaS5saXZlIiwKICAgICJpZCI6ICI3NTJhOTQwNC1jNzI5LTQ4NWUtOGVhNS1hY2IzZjRmYzgxODAiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogMTExMTEsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNS4xNjQuMTYzLjE0LTExODg0IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://752a9404-c729-485e-8ea5-acb3f4fc8180@hg17.leifengkeji.live:33387?allowInsecure=1&sni=hg17.leifengkeji.live#%F0%9F%87%B0%F0%9F%87%B7KR-15.164.103.48-0255
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:803#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0571
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@134.195.196.143:805#%F0%9F%87%A8%F0%9F%87%A6CA-134.195.196.143-15766
    vmess://ewogICAgImFkZCI6ICIxNDYuNTYuMTU1LjcwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJmOTc3MWMxOS1jOTFjLTQxYjUtOTA2NC04NzY4YjUxY2VjNmQiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTgwNTAsCiAgICAicHMiOiAi8J+HsPCfh7dLUi0xNDYuNTYuMTU1LjcwLTAzMjUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:801#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15760
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:803#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15754
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:802#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0537
    trojan://0Y9gOHSdRt@150.230.249.42:443?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-150.230.249.42-0291
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:805#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-0771
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:800#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15677
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:806#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0553
    vmess://ewogICAgImFkZCI6ICIxNTIuNjcuMjE4LjM4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiWW91VHViZS1hd2Vpa2VqaSIsCiAgICAiaWQiOiAiYjVlOTQ4MGEtYjdhYS00MGE0LWY5YTctNTI5OWI1ZTM2M2I0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE1Mi42Ny4yMTguMzgtMTU1NDUiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:800#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0543
    vmess://ewogICAgImFkZCI6ICI4LjIwOS4yMTguMTk1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAibGluZG8uY25hYmMuZXUub3JnIiwKICAgICJpZCI6ICJmNmQ3YjA3Mi1kZTAwLTQ1ZGMtOWUyNC00OWY4Y2Y0MzUzMGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvbGlub2QiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+Hr/Cfh7VKUC04LjIwOS4yMTguMTk1LTAzMjYiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICJ2bTE1LmxlaWZlbmdrZWppLmxpdmUiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ2bTE1LmxlaWZlbmdrZWppLmxpdmUiLAogICAgImlkIjogIjc1MmE5NDA0LWM3MjktNDg1ZS04ZWE1LWFjYjNmNGZjODE4MCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiAxMTExMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTU0LjE4MC4xMDEuNi0wMjkzIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICJhZWFkanBhZXMwMS54bi0tejRxNDhsY3ZwLmNvbSIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNob3V0aW5ndG91dGlhbzMuMTAwMTAuY29tIiwKICAgICJpZCI6ICIzZTgyMGViMC0zZjA2LTQzMzctYTRmYy0wYzNjN2MwZDNiNGQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaW1hZ2VzIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+Hr/Cfh7VKUC0xNzIuMTA0Ljc5Ljk2LTE2MTA3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNTIuNjcuMjE4LjM4IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTUyLjY3LjIxOC4zOCIsCiAgICAiaWQiOiAiYjVlOTQ4MGEtYjdhYS00MGE0LWY5YTctNTI5OWI1ZTM2M2I0IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE1Mi42Ny4yMTguMzgtMDIyNCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxMjkuMTU0LjU3LjEzNCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiY2FiYmRmNWQtM2NjYS00NjA1LWJhMWMtYzg5YTdkNWI0YzA3IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDI2MjgyLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTI5LjE1NC41Ny4xMzQtMDMyMyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTp2QXBZaUFnaHplc0g=@217.70.188.60:855#%F0%9F%87%AB%F0%9F%87%B7FR-217.70.188.60-15709
    vmess://ewogICAgImFkZCI6ICI1MS44OS40Mi4xNTQiLAogICAgImFpZCI6IDY0LAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI0MTgwNDhhZi1hMjkzLTRiOTktOWIwYy05OGNhMzU4MGRkMjQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvcGF0aC8xMjAyMTEzMzE0MjIiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HrPCfh6dHQi01MS44OS40Mi4xNTQtMjM3OSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJtNC40MDAxMDAxMC54eXoiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjU3NWU0ZDkyLTEwNTYtNDRjMi04Y2FjLTc1ZWYxYzg1OWFkNSIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAzNzEyMSwKICAgICJwcyI6ICLwn4ew8J+Ht0tSLTE0Ni41Ni4xMzMuMTA5LTAyODUiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:800#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10336
    vmess://ewogICAgImFkZCI6ICJ3d3cuYXB1bG5pb24uY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAid3d3LmFwdWxuaW9uLmNvbSIsCiAgICAiaWQiOiAiN2I4YzM3MGQtODYxMC00OTg4LWIwYTctY2RlNzRhYTA3MTNiIiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLzU4YTUzNDJmN2EvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTMyLjIyNi4xNzMuMTE4LTAzMzEiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNTIuNzAuMjM1LjIwNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiNzBkOTUzMDgtMmE2MS00ZjkzLWYxMzktOTEwM2QwNTg3ZmQ5IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDM1NDEyLAogICAgInBzIjogIvCfh7Dwn4e3S1ItMTUyLjcwLjIzNS4yMDctMDI3MSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiZG0udG91dGlhby5jb20iLAogICAgImlkIjogIjY4ZGY0ODM4LTQ2ZDAtNGI1Yi1jM2YwLWE0MGVjNzA2MzI0NSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi8iLAogICAgInBvcnQiOiA4MCwKICAgICJwcyI6ICLwn4e48J+HrFNHLTE4LjE0My4xMjMuMzUtMTU3MzMiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:804#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0555
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI2OGRmNDgzOC00NmQwLTRiNWItYzNmMC1hNDBlYzcwNjMyNDUiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvIiwKICAgICJwb3J0IjogODAsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0xOC4xNDMuMTIzLjM1LTAzMzciLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    trojan://bb5b1337-fa9e-4e00-b8c6-1110e626171d@159.223.89.239:443?allowInsecure=1#%F0%9F%87%B8%F0%9F%87%ACSG-159.223.89.239-0240
    vmess://ewogICAgImFkZCI6ICIxOC4xNDMuMTIzLjM1IiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTguMTQzLjEyMy4zNSIsCiAgICAiaWQiOiAiNjhkZjQ4MzgtNDZkMC00YjViLWMzZjAtYTQwZWM3MDYzMjQ1IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiLyIsCiAgICAicG9ydCI6IDgwLAogICAgInBzIjogIvCfh7jwn4esU0ctMTguMTQzLjEyMy4zNS0xNTcyMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    trojan://bb5b1337-fa9e-4e00-b8c6-1110e626171d@sg-01.tiktokcdn.top:443?allowInsecure=1#%F0%9F%87%B8%F0%9F%87%ACSG-159.223.89.239-0282
    vmess://ewogICAgImFkZCI6ICIxMzguMi40NC4yMTEiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICIiLAogICAgImlkIjogIjU5M2I4NTI1LTBjNDgtNGIwZi1kOWFmLTJkNzNhOTE0ODk3MyIsCiAgICAibmV0IjogInRjcCIsCiAgICAicGF0aCI6ICIiLAogICAgInBvcnQiOiAyMDA4MSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTEzOC4yLjQ0LjIxMS0wMjYzIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3LjYwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJhYzhlMjZmZS04MTUwLTRiNjAtYWU2NC04MmZjNzdlYmEyY2YiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTA2OSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNjAtMTM5OSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxNjcuMTcyLjY0LjExIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICI3NmEyNzZhMi0wZmMzLTRiZmItY2IwMC02Y2QyYTQzMDk2NzciLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTAwODYsCiAgICAicHMiOiAi8J+HuPCfh6xTRy0xNjcuMTcyLjY0LjExLTAyMzQiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    vmess://ewogICAgImFkZCI6ICIxNTIuNjkuMTk3LjYwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJhYzhlMjZmZS04MTUwLTRiNjAtYWU2NC04MmZjNzdlYmEyY2YiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMTA2OSwKICAgICJwcyI6ICLwn4ev8J+HtUpQLTE1Mi42OS4xOTcuNjAtMDMyMCIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICJzZzIwMi5oa2FhMC50ayIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNnMjAyLmhrYWEwLnRrIiwKICAgICJpZCI6ICJiZGY3OThmNC1hOTkwLTQ3NDMtZTliMi05Yzc4YmE1OGZiMDQiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaGthYTAiLAogICAgInBvcnQiOiAxMDE4LAogICAgInBzIjogIvCfh7jwn4esU0ctMTcyLjEwNC4xNjMuMjAyLTE3MDg3IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICJzZzIwMi5oa2FhMC50ayIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:809#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15659
    ss://YWVzLTI1Ni1jZmI6dkRTOUcycA==@185.4.65.6:21247#%F0%9F%87%B7%F0%9F%87%BARU-185.4.65.6-15714
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:803#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15657
    trojan://cb43b7c2-b744-41c5-bcc2-fd7467b332cf@jgwxn3.gaox.ml:443?allowInsecure=1#%F0%9F%87%A6%F0%9F%87%BAAU-140.238.205.173-14885
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:805#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0538
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:809#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15778
    trojan://c19d1432-8b3e-4818-8837-3d160cf65908@138.2.45.243:443?allowInsecure=1#%F0%9F%87%AF%F0%9F%87%B5JP-138.2.45.243-19249
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:809#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10334
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:804#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15656
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.154:802#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.154-15689
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:805#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15679
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTUzLjEwMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMi50cnVtcDIwMjMudXMiLAogICAgImlkIjogImJlZDNkODc2LTJkMjYtNGQ0ZC1iNzg5LTMwNjM0MzhlZTc3NCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTMuMTAyLTEwNTQiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:809#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15688
    vmess://ewogICAgImFkZCI6ICIxNi4xNjIuNTUuMTMwIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiMTYuMTYyLjU1LjEzMCIsCiAgICAiaWQiOiAiMTliOTVhMGUtZmZjZi0zMmVkLTg2NTYtNTJhZTEwMmE4YWQ4IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL255IiwKICAgICJwb3J0IjogNDQzMDAsCiAgICAicHMiOiAi8J+HrfCfh7BISy0xNi4xNjIuNTUuMTMwLTEyMzcxIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.221:812#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.221-0545
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:811#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15770
    vmess://ewogICAgImFkZCI6ICIxMzkuOTkuOTEuOTUiLAogICAgImFpZCI6IDMyLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICJjMDE1NjQ1MS00ZWZiLTQ1ZTItODRmYy04ZDMxNWM0NjUwZGIiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7jwn4esU0ctMTM5Ljk5LjkxLjk1LTAyMzIiLAogICAgInRscyI6ICIiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:810#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10335
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:812#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15693
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:808#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15691
    ss://YWVzLTI1Ni1jZmI6ZjYzZ2c4RXJ1RG5Vcm16NA==@213.183.59.214:9010#%F0%9F%87%B3%F0%9F%87%B1NL-213.183.59.214-17493
    vmess://ewogICAgImFkZCI6ICJzZy1vdmgxLnYyLXJheS5jb20iLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJzZy1vdmgxLnYyLXJheS5jb20iLAogICAgImlkIjogImE5NDgxNjAwLWVmMzYtNDAyYS1hMGU1LTU1NDdiZmQ3Yjg3YyIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9mYXN0c3NoL2ZnaGhoLzYzNDE5N2M0Y2RmODEvIiwKICAgICJwb3J0IjogNDQzLAogICAgInBzIjogIvCfh7jwn4esU0ctNTEuNzkuMTY0LjE0Ni0yNzc4IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    trojan://e05c749b-7c6b-41b8-9c71-9dcf685edf4a@152.67.162.166:443?allowInsecure=1&sni=content-provider22.cdn-delivery.akamaicd.com#%F0%9F%87%AE%F0%9F%87%B3IN-152.67.162.166-4645
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpxWUF0ODVTRkdWNTY=@185.77.217.217:443#%F0%9F%87%AB%F0%9F%87%AEFI-185.77.217.217-0797
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:811#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-10525
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:804#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15768
    vmess://ewogICAgImFkZCI6ICJmdWxsYWNjZXNzdG9rb3JlYW5uZXRzdWJub2RlMS5henVyZXdlYnNpdGVzLm5ldCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImZ1bGxhY2Nlc3N0b2tvcmVhbm5ldHN1Ym5vZGUxLmF6dXJld2Vic2l0ZXMubmV0IiwKICAgICJpZCI6ICIyNzRmMTFjNi1mNjliLTQwYjktODk2Ni1mMzllMDZlOTdiZTciLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvd3MiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+HsPCfh7dLUi01Mi4yMzEuMjAwLjE3OS01MDI5IiwKICAgICJ0bHMiOiAidGxzIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:809#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-10984
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.114.114.139:810#%F0%9F%87%BA%F0%9F%87%B8US-38.114.114.139-0772
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:804#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15753
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@196.247.59.156:803#%F0%9F%87%A8%F0%9F%87%A6CA-196.247.59.156-15777
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@162.251.61.47:800#%F0%9F%87%BA%F0%9F%87%B8US-162.251.61.47-15661
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:800#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-21268
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:805#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15767
    vmess://ewogICAgImFkZCI6ICIxNjguMTM4LjIwNy42NiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiOTA1Zjk5YjEtZTdiYS00NWUwLWFlNGQtYjBmZmRmMGFkMjQ1IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDIxMzY1LAogICAgInBzIjogIvCfh6/wn4e1SlAtMTY4LjEzOC4yMDcuNjYtMDI2NyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTopMU4xRTZ2MFNVX3JHVHBn@79.133.109.56:1036#%F0%9F%87%BA%F0%9F%87%B8US-79.133.109.56-15762
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:809#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15775
    vmess://ewogICAgImFkZCI6ICJ3d3cuZ292LmhrIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAidm4uY2xvdWRmbGFyZS5xdWVzdCIsCiAgICAiaWQiOiAiZGM4YjY0ZGItZWI2ZC00YmRmLTk4YjItMzE2MTUzMTliZWE4IiwKICAgICJuZXQiOiAid3MiLAogICAgInBhdGgiOiAiL2FyaWVzIiwKICAgICJwb3J0IjogMjA4NiwKICAgICJwcyI6ICLwn4+BUkVMQVktMTA0LjE2LjI0OS4xMzAtMTI5NSIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICIxODUuMjI1LjY5LjEzNCIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiM2MzYmZkNzUtZGMzMC00ZTc2LTg5NDAtNDdlMTEzN2UyMWY5IiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDQ1MDgxLAogICAgInBzIjogIvCfh63wn4e6SFUtMTg1LjIyNS42OS4xMzQtMDIyMyIsCiAgICAidGxzIjogIiIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:810#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15761
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@172.245.218.162:801#%F0%9F%87%BA%F0%9F%87%B8US-172.245.218.162-15719
    vmess://ewogICAgImFkZCI6ICJzZzExOC5oa2FhMC50ayIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogInNnMTE4LmhrYWEwLnRrIiwKICAgICJpZCI6ICI2NTJmNDI2My1iZDg2LTRiZjYtOWY3ZS1kMjVlNzUxNmZiNzIiLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvaGthYTAiLAogICAgInBvcnQiOiAxMzY5MSwKICAgICJwcyI6ICLwn4e48J+HrFNHLTE3Mi4xMDQuMTYzLjExOC0wMjQ4IiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:804#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10332
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:800#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15681
    vmess://ewogICAgImFkZCI6ICJ2c2cxLjBiYWQuY29tIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiJTdCJTIySG9zdCUyMjolMjJ2c2cxLjBiYWQuY29tJTIyJTdEIiwKICAgICJpZCI6ICI5MjcwOTRkMy1kNjc4LTQ3NjMtODU5MS1lMjQwZDBiY2FlODciLAogICAgIm5ldCI6ICJ3cyIsCiAgICAicGF0aCI6ICIvY2hhdCIsCiAgICAicG9ydCI6IDQ0MywKICAgICJwcyI6ICLwn4e48J+HrFNHLTE3MC4xODcuMTk2LjEyOC0xNTk4MSIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    vmess://ewogICAgImFkZCI6ICI4OS4yMDguMTA1LjYzIiwKICAgICJhaWQiOiAwLAogICAgImhvc3QiOiAiIiwKICAgICJpZCI6ICIyRjA5NDg0NS1FMkJELUVCRjctREVCNy05OTU5OTI0MzZGQUYiLAogICAgIm5ldCI6ICJ0Y3AiLAogICAgInBhdGgiOiAiIiwKICAgICJwb3J0IjogMjM0NTMsCiAgICAicHMiOiAi8J+Hs/Cfh7FOTC04OS4yMDguMTA1LjYzLTAzMDYiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@38.91.107.225:802#%F0%9F%87%BA%F0%9F%87%B8US-38.91.107.225-15692
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:812#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-0765
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:807#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20430
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:812#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15660
    trojan://3f087c04-44e6-4c96-a917-ca974de1212b@kr1.api-aws.com:443?allowInsecure=1#%F0%9F%87%B0%F0%9F%87%B7KR-146.56.176.239-15564
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.147.230:803#%F0%9F%87%BA%F0%9F%87%B8US-37.120.147.230-10337
    vmess://ewogICAgImFkZCI6ICIxNzIuNjQuMTUzLjEwMiIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogImNsYXNoMi50cnVtcDIwMjMudXMiLAogICAgImlkIjogImJlZDNkODc2LTJkMjYtNGQ0ZC1iNzg5LTMwNjM0MzhlZTc3NCIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9kb25ndGFpd2FuZy5jb20iLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTE3Mi42NC4xNTMuMTAyLTAyNTIiLAogICAgInRscyI6ICJ0bHMiLAogICAgInR5cGUiOiAiYXV0byIsCiAgICAic2VjdXJpdHkiOiAiYXV0byIsCiAgICAic2tpcC1jZXJ0LXZlcmlmeSI6IHRydWUsCiAgICAic25pIjogIiIKfQ==
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:805#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20428
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:801#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-2879
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:810#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20415
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:808#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20437
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:802#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20423
    vmess://ewogICAgImFkZCI6ICJ1bnVzMDEuYWpka2phbGpkai54eXoiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJ1bnVzMDEuYWpka2phbGpkai54eXoiLAogICAgImlkIjogIjk1ZTlmZGExLWRjNDgtM2JiZC04YTE1LWU2NTI4ODgyZWEzYiIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi82IiwKICAgICJwb3J0IjogMTA4MiwKICAgICJwcyI6ICLwn4e68J+HuFVTLTM4LjU0Ljk1LjE3OC01MjQxIiwKICAgICJ0bHMiOiAiIiwKICAgICJ0eXBlIjogImF1dG8iLAogICAgInNlY3VyaXR5IjogImF1dG8iLAogICAgInNraXAtY2VydC12ZXJpZnkiOiB0cnVlLAogICAgInNuaSI6ICIiCn0=
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@195.12.49.82:800#%F0%9F%87%AC%F0%9F%87%A7GB-195.12.49.82-20418
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:800#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-4617
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.159.30.61:808#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.30.61-0082
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@193.176.86.190:806#%F0%9F%87%A9%F0%9F%87%AADE-193.176.86.190-0969
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:801#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-0967
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:806#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-0763
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@37.120.219.218:801#%F0%9F%87%BA%F0%9F%87%B8US-37.120.219.218-15655
    vmess://ewogICAgImFkZCI6ICIyMTMuMjI2LjcxLjEyNyIsCiAgICAiYWlkIjogMCwKICAgICJob3N0IjogIiIsCiAgICAiaWQiOiAiMkYwOTQ4NDUtRTJCRC1FQkY3LURFQjctOTk1OTkyNDM2RkFGIiwKICAgICJuZXQiOiAidGNwIiwKICAgICJwYXRoIjogIiIsCiAgICAicG9ydCI6IDIzNDUzLAogICAgInBzIjogIvCfh6nwn4eqREUtMjEzLjIyNi43MS4xMjctNzkyNCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:807#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7529
    vmess://ewogICAgImFkZCI6ICJzZy5wcnByLmxpbmsiLAogICAgImFpZCI6IDAsCiAgICAiaG9zdCI6ICJzZy5wcnByLmxpbmsiLAogICAgImlkIjogImNlYTQyMTYxLWJkZGMtNDIzMC1hOWI5LWU0MzE4Nzk2N2ZmYSIsCiAgICAibmV0IjogIndzIiwKICAgICJwYXRoIjogIi9UZWxlZ3JhbS9TaGFyZUNlbnRyZVByby9ta25uaXgiLAogICAgInBvcnQiOiA0NDMsCiAgICAicHMiOiAi8J+PgVJFTEFZLTEwNC4yMS4zNS4yMTEtMTI1OCIsCiAgICAidGxzIjogInRscyIsCiAgICAidHlwZSI6ICJhdXRvIiwKICAgICJzZWN1cml0eSI6ICJhdXRvIiwKICAgICJza2lwLWNlcnQtdmVyaWZ5IjogdHJ1ZSwKICAgICJzbmkiOiAiIgp9
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:809#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7524
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:810#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-2099
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:804#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7527
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:808#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7521
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@51.159.30.61:809#%F0%9F%87%AB%F0%9F%87%B7FR-51.159.30.61-1423
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpHIXlCd1BXSDNWYW8=@185.104.184.78:802#%F0%9F%87%A9%F0%9F%87%B0DK-185.104.184.78-7526
    ss://Y2hhY2hhMjAtaWV0Zi1wb2x5MTMwNTpVbHRyQHIwMHRfMjAxNw==@138.68.248.130:811#%F0%9F%87%BA%F0%9F%87%B8US-138.68.248.130-0556

</details>

- you can import these 200 tested nodes using their subscription link into different clients. refer to `Instructions & Usage` section

### all nodes
merge nodes w/o dup: `5827`
- [Node link Mixed (V2ray)](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/sub_merge.txt)
- [Node link Yaml (Clash)](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge_yaml.yml)

#### all nodes separated by protoctol
- [VMESS](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/vmess.txt)
- [TROJAN](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/trojan.txt)
- [SSR](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/ssr.txt)
- [SHADOWSOCKS](https://raw.githubusercontent.com/mahdibland/ShadowsocksAggregator/master/sub/splitted/ss.txt)

#### provider config for clash 🐈‍⬛
> Configs with the "others" tag will proxy domestic services.

- [Clash Meta For Iran](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta.yml) (Recommended)
- [Clash Meta For China](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta-cn.yml) (Recommended)
- [Clash Meta For Others](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-meta-others.yml) (Recommended)

- [Clash For Iran](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider.yml)
- [Clash For China](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-cn.yml)
- [Clash For Others](https://cdn.jsdelivr.net/gh/mahdibland/V2RayAggregator@master/update/provider/provider-others.yml)


### node sources
- [pojiezhiyuanjun/freev2](https://github.com/pojiezhiyuanjun/freev2), number of nodes: `146`
- [Nodefree.org](https://github.com/Fukki-Z/nodefree), number of nodes: `20`
- [mianfeifq/share](https://github.com/mianfeifq/share), number of nodes: `68`
- [FiFier/v2rayShare](https://github.com/FiFier/v2rayShare), number of nodes: `21`
- [huanongkejizhijia/clashnode](https://github.com/huanongkejizhijia/clashnode), number of nodes: `21`
- [colatiger/v2ray-nodes](https://github.com/colatiger/v2ray-nodes), number of nodes: `121`
- [ssrsub/ssr](https://github.com/ssrsub/ssr), number of nodes: `683`
- [mahdibland/ShadowsocksAggregator](https://github.com/mahdibland/ShadowsocksAggregator), number of nodes: `200`
- [iwxf/free-v2ray](https://github.com/iwxf/free-v2ray), number of nodes: `39`
- [DoveBoy/Vmess-Actions](https://github.com/ldir92664/Vmess-Actions), number of nodes: `105`
- [gooooooooooooogle/Clash-Config](https://github.com/gooooooooooooogle/Clash-Config), number of nodes: `1`
- [Jsnzkpg/Jsnzkpg](https://github.com/Jsnzkpg/Jsnzkpg), number of nodes: `16`
- [ermaozi/get_subscribe](https://github.com/ermaozi/get_subscribe), number of nodes: `21`
- [wrfree/free](https://github.com/wrfree/free), number of nodes: `51`
- [anaer/Sub](https://github.com/anaer/Sub), number of nodes: `954`
- [aiboboxx/v2rayfree](https://github.com/aiboboxx/v2rayfree), number of nodes: `30`
- [Pawdroid/Free-servers](https://github.com/Pawdroid/Free-servers), number of nodes: `19`
- [Rokate/Proxy-Sub](https://github.com/Rokate/Proxy-Sub), number of nodes: `69`
- [misersun/config003-002](https://github.com/misersun/config003), number of nodes: `217`
- [clash.221207.xyz/pubclashyaml](https://clash.221207.xyz/pubclashyaml), number of nodes: `1205`
- [mfuu/v2ray](https://github.com/mfuu/v2ray), number of nodes: `359`
- [freefq/free](https://github.com/freefq/free), number of nodes: `16`
- [xiyaowong/freeFQ](https://github.com/xiyaowong/freeFQ), number of nodes: `156`
- [yaney01/Yaney01](https://github.com/yaney01/Yaney01), number of nodes: `66`
- [YasserDivaR/pr0xy](https://github.com/YasserDivaR/pr0xy), number of nodes: `1385`
- [peasoft/NoMoreWalls](https://github.com/peasoft/NoMoreWalls), number of nodes: `182`
- [mahdibland/get_v2](https://github.com/mahdibland/get_v2), number of nodes: `2383`
- [free.jingfu.cf/clash](https://free.jingfu.cf/clash), number of nodes: `210`
- [jikelonglie/meskell](https://github.com/jikelonglie/meskell), number of nodes: `9`
- [freebaipiao/freebaipiao](https://github.com/freebaipiao/freebaipiao), number of nodes: `6`
- [huwo1/proxy_nodes](https://bitbucket.org/huwo1/proxy_nodes/src/main), number of nodes: `183`
- [lisylva-lee/v2dyku](https://github.com/lisylva-lee/v2dyku), number of nodes: `5`
- [budamu/clashconfig](https://github.com/budamu/clashconfig), number of nodes: `142`
- [MOnday9907/v2ray](https://github.com/MOnday9907/v2ray), number of nodes: `8`
- [adminaliang/v2ray](https://github.com/adminaliang/v2ray), number of nodes: `16`
- [Jia-Pingwa/free-v2ray-merge](https://github.com/Jia-Pingwa/free-v2ray-merge), number of nodes: `327`
- [Lewis-1217/FreeNodes](https://github.com/Lewis-1217/FreeNodes), number of nodes: `39`
- [youlianboshi.netlify.app](https://youlianboshi.netlify.app), number of nodes: `7`
- [jiang.netlify.app](https://jiang.netlify.app), number of nodes: `46`
- [learnhard-cn/free_proxy_ss](https://github.com/learnhard-cn/free_proxy_ss), number of nodes: `116`
- [SnapdragonLee/SystemProxy](https://github.com/SnapdragonLee/SystemProxy), number of nodes: `239`
- [free.iam7.tk/clash](https://free.iam7.tk/clash), number of nodes: `344`
- [sub.pmsub.me/base64](https://sub.pmsub.me/base64), number of nodes: `2`
- [hermanb001/ProxyTest](https://github.com/hermanb001/ProxyTest), number of nodes: `1743`
- [LonUp/NodeList](https://github.com/LonUp/NodeList), number of nodes: `1451`

## Softwares

### Best Clients For Each OS

|    OS   |              Best Client               | Alternatives |
|:-------:|:--------------------------------------:|:------------:|
|   IOS   |        Quantumult - Shadowrocket       |  NapsternetV |
| Android |Surfboard - Clash For Android - Matsuri |    V2rayNg   |
| Windows |   Clash For Windows - V2rayN - Nekoray |    Qv2ray    |
|  Linux  |           Clash For Windows            |    Qv2ray    |
|  MacOS  |           Clash For Windows            |    Qv2ray    |

### Desktop Clients

|                              MacOS                               |                              Linux                               |                                       Windows                                       | Brief description                                                                                         |
| :--------------------------------------------------------------: | :--------------------------------------------------------------: | :---------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------- |
| [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW](https://github.com/Fndroid/clash_for_windows_pkg/releases) | [CFW(Clash For Windows)](https://github.com/Fndroid/clash_for_windows_pkg/releases) | SS, SSR, Trojan, Vmess, VLESS protocol support, strong policy offload capability.                                         |
|       [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)        |       [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)        |                 [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)                 | SS, SSR, Trojan, Vmess, VLESS, Trojan-Go protocol support (relevant plugins need to be installed).                            |
|                                ×                                 |                                ×                                 |                 [V2rayN](https://github.com/2dust/v2rayN/releases)                  | SS, Trojan, Vmess, VLESS protocol support, with speed measurement, delay measurement function, support subscription, QR code, clipboard import and manual configuration.  |
|                                ×                                 |                                ×                                 |               [WinXray](https://github.com/TheMRLL/winxray/releases)                | SS, SSR, Trojan, Vmess, VLESS protocol support, support automatic connection to the fastest node.                                   |
|                                ×                                 |                                ×                                 | [Shadowsocks-windows](https://github.com/shadowsocks/shadowsocks-windows/releases)  | SS protocol support, SS dedicated client.                                                                    |
|                                ×                                 |                                ×                                 |  [ShadowsocksR-windows](https://github.com/HMBSbige/ShadowsocksR-Windows/releases)  | SSR protocol support, SSR dedicated client.                                                                   |
|                  [Surge](https://nssurge.com/)                   |                                ×                                 |                                          ×                                          | SS, Trojan, Vmess protocol support, well-known network debugging tools, powerful strategy offloading ability, need to pay.                         |
|     [ClashX](https://github.com/yichengchen/clashX/releases)     |                                ×                                 |                                          ×                                          | SS, SSR, Trojan, Vmess protocol support, occupy less resources.                                                  |
|        [V2rayU](https://github.com/yanue/V2rayU/releases)        |                                ×                                 |                                          ×                                          | SS, Trojan, Vmess protocol support, support subscription, QR code, clipboard import, manual configuration, QR code sharing, similar to V2RayN. |
|       [V2rayA](https://github.com/v2rayA/v2rayA/releases/)       |       [V2rayA](https://github.com/v2rayA/v2rayA/releases/)       |                [V2rayA](https://github.com/v2rayA/v2rayA/releases/)                 | V2Ray, Xray, SS, SSR, Trojan support, subscription and manual config.  |

### Mobile Clients

|                               iOS/iPadOS                                |                                      Android                                       | Brief description                                                                                                                                                  |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------------------: | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)  |  [Shadowrocket](https://play.google.com/store/apps/details?id=com.v2cross.proxy)   | SS, SSR, Trojan, Vmess, VLESS protocol support, the iOS side needs to be purchased in the non-country App Store, the US price is $2.99; the Android side is not the same author as the iOS side, does not support the SSR protocol, free and built-in free nodes. |
|                      [Surge](https://nssurge.com/)                      |                                         ×                                          | SS, Trojan, Vmess protocol support, well-known network debugging tools on the iOS side, chargeable.                                                                                              |
| [Quantumult X](https://apps.apple.com/us/app/quantumult-x/id1443988620) |                                         ×                                          |                                                                                 |
| [Potatso Lite](https://apps.apple.com/us/app/potatso-lite/id1239860606) |                                         ×                                          | SS, SSR protocol support, need to be purchased in the non-country AppStore, free.                                                                                                        |
|                                    ×                                    |    [Surfboard](https://play.google.com/store/apps/details?id=com.getsurfboard)     | SS, SSR, Vmess Protocol support, Android network debugging software, compatible with Surge 2 configuration.                                                                                          |
|                                    ×                                    |    [CFA(Clash For Android)](https://github.com/Kr328/ClashForAndroid/releases)     | SS, SSR, Trojan, Vmess Protocol support.                                                                                                                         |
|                                    ×                                    |             [SagerNet](https://github.com/SagerNet/SagerNet/releases)              | SS, SSR, Trojan, Vmess, VLESS Protocol support.                                                                                                                  |
|                                    ×                                    | [Shadowsocks-android](https://github.com/shadowsocks/shadowsocks-android/releases) | SS protocol support, Android-specific SS client.                                                                                                                         |
|                                    ×                                    | [ShadowsocksR-android](https://github.com/HMBSbige/ShadowsocksR-Android/releases)  | SSR protocol support, Android-specific SSR client.                                                                                                                       |
|                                    ×                                    |                [V2rayNG](https://github.com/2dust/v2rayNG/releases)                | SS, Trojan, Vmess, VLESS protocol support, v2ray kernel.                                                                                                           |

### Credit: 
- [alanbobs999](https://github.com/alanbobs999)
- [PersianBlocker](https://github.com/MasterKia/PersianBlocker)
- [iran-hosted-domains](https://github.com/bootmortis/iran-hosted-domains)
