sudo ufw allow 80
sudo ufw allow 443

sudo apt install letsencrypt

sudo certbot certonly --standalone --agree-tos --preferred-challenges http -d domain-name.com

openssl pkcs12 -export -out ciphermail.p12 -inkey myKey.pem -in cert.pem

scp username@hostname:/path/to/remote/file /path/to/local/file