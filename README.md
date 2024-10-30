# RC-overleaf

1. Install Ubuntu.

2. Update system.
```
sudo apt update && sudo apt upgrade -y
```

3. Download and Install Docker.

3.1 Set up Docker's apt repository.
```
# Add Docker's official GPG key
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```
  
3.2 Install the Docker packages.
```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

3.3 Verify that the Docker Engine installation is successful by running the hello-world image.
```
sudo docker run hello-world
```

Optional:
3.4 Create the docker group.
```
sudo groupadd docker
```

3.5 Add your user to the docker group.
```
sudo usermod -aG docker $USER
```

3.6 Log out and log back in so that your group membership is re-evaluated.
You can also run the following command to activate the changes to groups:
```
newgrp docker
```

3.7 Verify that you can run docker commands without sudo.
```
docker run hello-world
```

4. Download and Install Overleaf-toolkit.
```

```

5. Update Latex packages.
```

```
