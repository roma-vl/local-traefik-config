### Додати в /etc/hosts якщо нема

127.0.0.1   dev.filkx.com
127.0.0.1   dev.auction.filkx.com
127.0.0.1   dev.api.auction.filkx.com
127.0.0.1   dev.rtmp.live.filkx.com
127.0.0.1   dev.board.filkx.com
127.0.0.1   dev.manager.filkx.com
127.0.0.1   dev.live.filkx.com
127.0.0.1   dev.api.live.filkx.com



sudo apt install libnss3-tools
curl -JLO "https://dl.filippo.io/mkcert/latest?for=linux/amd64"
chmod +x mkcert-v*-linux-amd64
sudo mv mkcert-v*-linux-amd64 /usr/local/bin/mkcert
mkcert -install

mkcert dev.auction.filkx.com dev.api.auction.filkx.com dev.live.filkx.com dev.api.live.filkx.com dev.rtmp.live.filkx.com dev.filkx.com

і перемістити сертифікати в docker/certs


