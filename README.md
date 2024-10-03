Prerequisites
Make sure you have the following installed on your machine:

Docker
Docker Compose

# Update your package database
sudo apt update

# Install Docker
sudo apt install docker.io -y

# Start Docker and enable it to start at boot
sudo systemctl start docker
sudo systemctl enable docker

docker --version
Create a .env file in the root of your project and add the following environment variables:

MONGO_USERNAME=siva
MONGO_PASSWORD=siva
MONGO_PORT=27017
MONGO_DB=sharkinfo

Ensure that the wait-for.sh script has the correct execution permissions. Run the following command:

chmod +x wait-for.sh

Use Docker Compose to build and run the containers:

docker compose up -d
