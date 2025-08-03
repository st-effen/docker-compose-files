# HowTo create a local home net bridge with ipv6

docker network create -d macvlan --ipv6 --subnet=192.168.3.0/24 --gateway=192.168.3.1 --subnet=fd01::/64 --gateway=fd01::1  -o parent=eno1.2 -o macvlan_mode=bridge macvlan1
