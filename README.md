REVERSE PROXY SETUP AND UPDATES

This is my first stable Docker project, and it is working as expected. Enjoy! :)

REQUIREMENTS

WSL 2

Docker Desktop

Git (optional, if you want to clone the repository)

STEP-BY-STEP GUIDE

Make sure to use the traefik-proxy-01 project folder.

DOWNLOAD THE PROJECT

Download the ZIP file or clone the repository using Git:

git clone <repository-url>

GENERATE AN SSL CERTIFICATE

Inside the certs folder, generate a self-signed SSL certificate and private key:

openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout privkey.key -out pubkey.crt

START THE PROJECT

Make sure you are inside the project folder, then run:

docker compose up --build

ACCESS THE APPLICATION

Open your favorite web browser and navigate to:

http://localhost/

Your reverse proxy should now be up and running!
