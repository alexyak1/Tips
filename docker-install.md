# Install docker to Ubuntu/Debian

### Uninstall old Docker versions (if any)

`sudo apt-get remove docker docker-engine docker.io`

### Update package index

`sudo apt-get update`

### Install required packages
`sudo apt-get install -y apt-transport-https ca-certificates curl gnupg lsb-release`

### Add Docker’s official GPG key
`curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg`

### Set up the stable repository
`echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/debian $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null`

### Update package index again
`sudo apt-get update`

### Install Docker Engine
`sudo apt-get install -y docker-ce docker-ce-cli containerd.io`

### Verify Docker Installation
`sudo docker run hello-world`
