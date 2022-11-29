if timeout accured check security groups rules.  

To add ssh key and connect: 

```bash
sudo chmod 0400 <pemfile>
sudo ssh -i <pemfile> ec2-user@instancepublicid
```
