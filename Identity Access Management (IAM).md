---


---

<h1 id="iam---identity-access-management">IAM - Identity Access Management</h1>
<p><strong>IAM</strong> - Who, What (<em>can they do</em>), Resource (<em>on what</em>)</p>
<pre><code>Organisation Node
       |
    Folders
       |
    Projects
       |
   Resources
</code></pre>
<h2 id="projects">Projects</h2>
<ul>
<li>
<p><strong>Project Id</strong> - Globally unique immutable but can be edited during generation.</p>
</li>
<li>
<p><strong>Project Name</strong> - Mutable.</p>
</li>
<li>
<p><strong>Project Number</strong> - Globally unique - auto generated.</p>
</li>
</ul>
<h2 id="roles">Roles</h2>
<p>3 types of Role:</p>
<ul>
<li>
<p><strong>Primitive</strong> (viewer, editor, owner)</p>
<ul>
<li>Affect all resources in a project.</li>
</ul>
</li>
<li>
<p><strong>Predefined</strong></p>
</li>
<li>
<p><strong>Customer</strong></p>
<ul>
<li>Cannot assign these at a folder level (only Project or Org’).</li>
</ul>
</li>
</ul>
<h2 id="service-accounts">Service Accounts</h2>
<p>Service accounts are both an identity and a resource</p>

