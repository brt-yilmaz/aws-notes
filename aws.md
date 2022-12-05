if timeout accured check security groups rules.  

To add ssh key and connect: 

```bash
sudo chmod 0400 <pemfile>
sudo ssh -i <pemfile> ec2-user@instancePublicId
```
add instance iam role via action>security>modify iam

> search how can i use EBS volume via local terminal.  

Volumes and instances must be in same availability zone. You can set this while creating volumes.  

Root volumes has a default option to delete volumes when instance terminated. Be careful about that. You can set this when you create an instance in EBS Advance section.  

You can create a snapshot for the volumes, go to EBS > Volumes > Actions > Create Snapshot
after that you can find it in EBS > Snapshot section. You can copy it for another zone.  

You must be set retention rules before you create a snapshot.  
