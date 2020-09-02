# Compute Engine - Managed VMs

Persistent disks - standard or SSD
Local SSD non persistent.
Can define a startup script.
Take snapshot as backups or migration tools
Preemptible available


```
> gcloud compute zones list
> gcloud config set compute/zone us-central-c
> gcloud create instances create "my-vm" --machine type "n1-standard1" \
  --image-project "debian-cloud" --image "debian-9-st..." --subnet "default"
```


can ssh in the cloud shell
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcwMDA2NjA1OV19
-->