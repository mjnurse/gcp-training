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
	-	Location (region / multi region)
	-	IAM policies or Access Control Lists
	-	Object versioning setting
	-	Object lifecycle management rules
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY5MzEyNzc2MywxODczMDI4MzE5LC03OT
QwNjU2NzFdfQ==
-->