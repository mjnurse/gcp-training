---


---

<h1 id="compute-engine-gce---managed-vms">Compute Engine (GCE) - Managed VMs</h1>
<p>Persistent disks - standard or SSD<br>
Local SSD non persistent.<br>
Can define a startup script.<br>
Take snapshot as backups or migration tools<br>
Preemptible available</p>
<pre><code>&gt; gcloud compute zones list
&gt; gcloud config set compute/zone us-central-c
&gt; gcloud create instances create "my-vm" --machine type "n1-standard1" \
  --image-project "debian-cloud" --image "debian-9-st..." --subnet "default"
</code></pre>
<p>can ssh in the cloud shell</p>

