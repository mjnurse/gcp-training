# Google Cloud Storage (GCS)

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

### Integrated with
-	**Big Query** - import and export tables.
-	**App engine** - obj' storage, logs and backups.
-	**Compute Engine** - startup scripts, images and general objects.
-	**Cloud SQL** - import and export tables.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc0MjU1MDcyN119
-->