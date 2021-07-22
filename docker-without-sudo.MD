# How to run docker comand without sudo

### Add user group
`sudo groupadd docker`

### Add user to this group
`sudo usermod -aG docker $USER`
### Give proper permissions to make it work
`sudo chown root:docker /var/run/docker.sock` <br/>
`sudo chown -R root:docker /var/run/docker`
