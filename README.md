
# Wireguard Server configs




## Useful commands
To create keys
```bash
  wg genkey | tee server-privatekey | wg pubkey > server-publickey
```
To view keys
```bash
  tail -n +1 server-privatekey server-publickey
```
to get public ip address
```bash
  curl ipconfig.io
```
### service commands
```bash
  systemctl enable wg-quick@wg0
```
```bash
  systemctl start wg-quick@wg0
```
```bash
  systemctl stop wg-quick@wg0
```
```bash
  systemctl status wg-quick@wg0
```

## References
[Oracle Cloud Wireguard Setp by step](https://www.reddit.com/r/WireGuard/comments/1baeuyx/wireguard_oracle_cloud_step_by_step/)

[Wireguard Server setup on oracle cloud](https://techtutelage.net/?p=303)

[DigitialOcean Tutorial](https://www.digitalocean.com/community/tutorials/how-to-set-up-wireguard-on-ubuntu-20-04#step-6-starting-the-wireguard-server)

[Wireguard Server Setup - 1](https://docs.vultr.com/how-to-install-wireguard-vpn-on-ubuntu-24-04#manage-wireguard-vpn-server-system-processes)

[Wireguard Server Setup - 2](https://www.ntkernel.com/setting-up-wireguard-on-oracle-cloud-overcoming-nat-and-routing-challenges/)

[Oracle iptables information](https://blogs.oracle.com/developers/post/enabling-network-traffic-to-ubuntu-images-in-oracle-cloud-infrastructure)