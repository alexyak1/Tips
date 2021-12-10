# How to run docker comand without sudo

### Add user group
`sudo groupadd docker`

### Add user to this group
`sudo usermod -aG docker $USER`
### Give proper permissions to make it work
`sudo chown root:docker /var/run/docker.sock` <br/>
`sudo chown -R root:docker /var/run/docker`

Logging out and logging back in is required because the group change will not have an effect unless your session is closed.
