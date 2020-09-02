---


---

<h1 id="google-cloud-storage-gcs">Google Cloud Storage (GCS)</h1>
<ul>
<li>Binary large object storage.</li>
<li>No capacity management.</li>
<li>Access via unique key (eg URL).</li>
<li>Not a file system - object can be call files.   Do not use as a file system.</li>
<li>Immutable - never edit always replace with new.</li>
<li>Organised by buckets.
<ul>
<li>Globally unique name.</li>
<li>Storage Class.</li>
<li>Location (region / multi region).</li>
<li>IAM policies or ACLs (Access Control Lists).</li>
<li>Object versioning setting.</li>
<li>Object lifecycle management rules (<em>eg delete obj’s older than 365 days, only keep 3 versions</em>)</li>
</ul>
</li>
</ul>
<h3 id="storage-classes">Storage Classes</h3>
<ul>
<li><strong>Multi-Regional</strong> - Most frequent access - avail SLA 99.95% - Content storage and delivery.
<ul>
<li>Two locations &gt; 160km.</li>
<li>Main cost per GB per month.</li>
</ul>
</li>
<li><strong>Regional</strong> - Frequent access in a region - avail SLA 99.90% - In region analytics / transcoding.</li>
<li><strong>Nearline</strong> - Access avg. &lt; once a month - avail SLA 99.00% - backups, long tail content.
<ul>
<li>Cost includes per GB transferred.</li>
</ul>
</li>
<li><strong>Coldline</strong> - Access avg. &lt; once a year - avail SLA 99.00% - archiving, DR.
<ul>
<li>Main cost per GB transferred.</li>
<li>Min 90 days storage.</li>
</ul>
</li>
</ul>
<h3 id="integrated-with">Integrated with</h3>
<ul>
<li><strong>Big Query</strong> - import and export tables.</li>
<li><strong>App engine</strong> - obj’ storage, logs and backups.</li>
<li><strong>Compute Engine</strong> - startup scripts, images and general objects.</li>
<li><strong>Cloud SQL</strong> - import and export tables.</li>
</ul>

