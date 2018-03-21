tshark tcp port 80 or tcp port 443 -V -R "http.request || http.response" -2 -i ens33
sudo tshark -i eth0  -d tcp.port==3306,mysql -T fields -e mysql.query 'port 3306'
sudo tshark host 10.66.177.125  # issued at uatapp01 to find out the traffic coming from uatdb01

tshark -i < > -d tcp.port == 1433 && ip.addr == <sql server ip>

