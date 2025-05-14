# cyberlabcodes
test
deb http://http.kali.org/kali kali-rolling main contrib non-free

sudo sysctl -w net.ipv4.ip_forward=1

cat /proc/sys/net/ipv4/ip_forward

sudo iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE
sudo iptables -A FORWARD -i eth0 -j ACCEPT
