### Додати в /etc/hosts якщо нема
127.0.0.1   dev.auction.filkx.com
127.0.0.1   dev.api.auction.filkx.com
127.0.0.1   dev.board.filkx.com
127.0.0.1   dev.manager.filkx.com
127.0.0.1   dev.filkx.com


sudo apt install libnss3-tools
curl -JLO "https://dl.filippo.io/mkcert/latest?for=linux/amd64"
chmod +x mkcert-v*-linux-amd64
sudo mv mkcert-v*-linux-amd64 /usr/local/bin/mkcert
mkcert -install

mkcert dev.auction.filkx.com dev.api.auction.filkx.com

і перемістити сертифікати в docker/certs
