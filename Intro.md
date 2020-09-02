#  GCP Training

##  What is Cloud Computing?

5 features of Cloud Computing
-	On demand, self service.
-	Broad network access.
-	Resource pooling.
-	Rapid elasticity.
-	Measure service (PAYG).

Acronyms
-	Iaas - Infrastructure as a service.
-	Paas - Platform as a service.
-	Saas - Software as a service.

##  Regions / Zones

-	Zone is a deployment area (europe-west2-a).
-	Regions contain many zones.
-	Zone -> Zone < 5ms latency.
-	Multi Region - stored redundantly in 2 locations >= 160km apart

##  Billing - Sub Hour Increments

Discount:

-	Sustained use (auto when used > 25% a month).
-	Committed use.
-	Preemptable machines.
-	Custom VM's.

##  Multi-Layered Security

-	Titan security chip.
-	Machine cryptographic signatures.
-	Disk HW encryption.
-	Google Front End - check for correct certificates etc.

##  Billing

-	Budgets and alerts
-	Billing exports
-	Reports
-	Quotas
-	Allocation eg < 5 networks

## Storage Options

### Cloud Storage (GCS)

-	Binary large object storage.
-	No capacity management.
-	Access via unique key (eg URL).
-	Not a file system - object can be call files.   Do not use as a file system.
-	Immutable - never edit always replace with new.
-	Organised by buckets.
	-	Globally unique name.
	-	Storage Class.
	-	Location (region / multi region).
	-	IAM policies or ACLs (Access Control Lists).
	-	Object versioning setting.
	-	Object lifecycle management rules (*eg delete obj's older than 365 days, only keep 3 versions*)

### Storage Classes

-	**Multi-Regional** - Most frequent access - avail SLA 99.95% - Content storage and delivery.
	-	Two locations > 160km.
	-	Main cost per GB per month. 
-	**Regional** - Frequent access in a region - avail SLA 99.90% - In region analytics / transcoding.
-	**Nearline** - Access avg. < once a month - avail SLA 99.00% - backups, long tail content.
	-	Cost includes per GB transferred.
-	**Coldline** - Access avg. < once a year - avail SLA 99.00% - archiving, DR.
	-	Main cost per GB transferred.
	-	Min 90 days storage.

Integrated with
-	Import / export Big Query
-	App engine - obj' storage, logs and backups
-	Compute Engine - 




<!--stackedit_data:
eyJoaXN0b3J5IjpbOTAxODU4OTg0LDE4NzMwMjgzMTksLTc5ND
A2NTY3MV19
-->