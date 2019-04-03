# Docker-ssh

An SSHd service in a Docker container

Set USER_PASSWORD environment variable

To run container:
```
docker run --name sshd -p 2222:22 -d -t -e USER_ID=1000 -e GROUP_ID=1000 -v -e USER_PASSWORD=mypassword /part/to/project:/home/project/ mazhuravlev/sshd
```

To SSH into your container:
```
ssh project@localhost -p 2222
```