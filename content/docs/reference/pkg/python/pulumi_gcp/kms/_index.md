---
title: Module kms
---

<div class="section" id="kms">
<h1>kms<a class="headerlink" href="#kms" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-gcp/issues">pulumi/pulumi-gcp repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/issues">terraform-providers/terraform-provider-google repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_gcp.kms"></span><dl class="class">
<dt id="pulumi_gcp.kms.AwaitableGetKMSCryptoKeyResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">AwaitableGetKMSCryptoKeyResult</code><span class="sig-paren">(</span><em>key_ring=None</em>, <em>labels=None</em>, <em>name=None</em>, <em>purpose=None</em>, <em>rotation_period=None</em>, <em>self_link=None</em>, <em>version_templates=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.AwaitableGetKMSCryptoKeyResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.AwaitableGetKMSCryptoKeyVersionResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">AwaitableGetKMSCryptoKeyVersionResult</code><span class="sig-paren">(</span><em>algorithm=None</em>, <em>crypto_key=None</em>, <em>protection_level=None</em>, <em>public_key=None</em>, <em>state=None</em>, <em>version=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.AwaitableGetKMSCryptoKeyVersionResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.AwaitableGetKMSKeyRingResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">AwaitableGetKMSKeyRingResult</code><span class="sig-paren">(</span><em>location=None</em>, <em>name=None</em>, <em>project=None</em>, <em>self_link=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.AwaitableGetKMSKeyRingResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.AwaitableGetKMSSecretResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">AwaitableGetKMSSecretResult</code><span class="sig-paren">(</span><em>ciphertext=None</em>, <em>crypto_key=None</em>, <em>plaintext=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.AwaitableGetKMSSecretResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.CryptoKey">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">CryptoKey</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>key_ring=None</em>, <em>labels=None</em>, <em>name=None</em>, <em>purpose=None</em>, <em>rotation_period=None</em>, <em>version_template=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKey" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">CryptoKey</span></code> represents a logical key that can be used for cryptographic operations.</p>
<blockquote>
<div><strong>Note:</strong> CryptoKeys cannot be deleted from Google Cloud Platform.
Destroying a CryptoKey will remove it from state
and delete all CryptoKeyVersions, rendering the key unusable, but <em>will
not delete the resource on the server.</em> When this provider destroys these keys,
any data previously encrypted with these keys will be irrecoverable.
For this reason, it is strongly recommended that you add lifecycle hooks
to the resource to prevent accidental destruction.</div></blockquote>
<p>To get more information about CryptoKey, see:</p>
<ul class="simple">
<li><a class="reference external" href="https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys">API documentation</a></li>
<li>How-to Guides<ul>
<li><a class="reference external" href="https://cloud.google.com/kms/docs/creating-keys#create_a_key">Creating a key</a></li>
</ul>
</li>
</ul>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key.html.markdown</a>.</div></blockquote>
<dl class="staticmethod">
<dt id="pulumi_gcp.kms.CryptoKey.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>key_ring=None</em>, <em>labels=None</em>, <em>name=None</em>, <em>purpose=None</em>, <em>rotation_period=None</em>, <em>self_link=None</em>, <em>version_template=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKey.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing CryptoKey resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.CryptoKey.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKey.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.CryptoKey.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKey.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">CryptoKeyIAMBinding</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>crypto_key_id=None</em>, <em>members=None</em>, <em>role=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>Allows creation and management of a single binding within IAM policy for
an existing Google Cloud KMS crypto key.</p>
<blockquote>
<div><dl class="docutils">
<dt><strong>Note:</strong> On create, this resource will overwrite members of any existing roles.</dt>
<dd>Use <code class="docutils literal notranslate"><span class="pre">import</span></code> and inspect the preview output to ensure
your existing members are preserved.</dd>
</dl>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>crypto_key_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The crypto key ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}/{crypto_key_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}/{crypto_key_name}</span></code>.
In the second form, the provider’s project setting will be used as a fallback.</li>
<li><strong>members</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of users that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.CryptoKeyIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_binding.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding.crypto_key_id">
<code class="descname">crypto_key_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding.crypto_key_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The crypto key ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}/{crypto_key_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}/{crypto_key_name}</span></code>.
In the second form, the provider’s project setting will be used as a fallback.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the crypto key’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding.members">
<code class="descname">members</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding.members" title="Permalink to this definition">¶</a></dt>
<dd><p>A list of users that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.CryptoKeyIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>crypto_key_id=None</em>, <em>etag=None</em>, <em>members=None</em>, <em>role=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing CryptoKeyIAMBinding resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] crypto_key_id: The crypto key ID, in the form</p>
<blockquote>
<div><code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}/{crypto_key_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}/{crypto_key_name}</span></code>.
In the second form, the provider’s project setting will be used as a fallback.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>etag</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – (Computed) The etag of the crypto key’s IAM policy.</li>
<li><strong>members</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A list of users that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.CryptoKeyIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_binding.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.CryptoKeyIAMBinding.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">CryptoKeyIAMMember</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>crypto_key_id=None</em>, <em>member=None</em>, <em>role=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember" title="Permalink to this definition">¶</a></dt>
<dd><p>Allows creation and management of a single member for a single binding within
the IAM policy for an existing Google Cloud KMS crypto key.</p>
<blockquote>
<div><dl class="docutils">
<dt><strong>Note:</strong> This resource <em>must not</em> be used in conjunction with</dt>
<dd><code class="docutils literal notranslate"><span class="pre">google_kms_crypto_key_iam_policy</span></code> or they will fight over what your policy
should be. Similarly, roles controlled by <code class="docutils literal notranslate"><span class="pre">kms.CryptoKeyIAMBinding</span></code>
should not be assigned to using <code class="docutils literal notranslate"><span class="pre">kms.CryptoKeyIAMMember</span></code>.</dd>
</dl>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>crypto_key_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}/{crypto_key_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}/{crypto_key_name}</span></code>. In the second form,
the provider’s project setting will be used as a fallback.</li>
<li><strong>member</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The user that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_member.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember.crypto_key_id">
<code class="descname">crypto_key_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember.crypto_key_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}/{crypto_key_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}/{crypto_key_name}</span></code>. In the second form,
the provider’s project setting will be used as a fallback.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the project’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember.member">
<code class="descname">member</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember.member" title="Permalink to this definition">¶</a></dt>
<dd><p>The user that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>crypto_key_id=None</em>, <em>etag=None</em>, <em>member=None</em>, <em>role=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing CryptoKeyIAMMember resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] crypto_key_id: The key ring ID, in the form</p>
<blockquote>
<div><code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}/{crypto_key_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}/{crypto_key_name}</span></code>. In the second form,
the provider’s project setting will be used as a fallback.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>etag</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – (Computed) The etag of the project’s IAM policy.</li>
<li><strong>member</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The user that the role should apply to. For more details on format and restrictions see <a class="reference external" href="https://cloud.google.com/billing/reference/rest/v1/Policy#Binding">https://cloud.google.com/billing/reference/rest/v1/Policy#Binding</a></li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_crypto_key_iam_member.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.CryptoKeyIAMMember.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.CryptoKeyIAMMember.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">GetKMSCryptoKeyResult</code><span class="sig-paren">(</span><em>key_ring=None</em>, <em>labels=None</em>, <em>name=None</em>, <em>purpose=None</em>, <em>rotation_period=None</em>, <em>self_link=None</em>, <em>version_templates=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getKMSCryptoKey.</p>
<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyResult.purpose">
<code class="descname">purpose</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyResult.purpose" title="Permalink to this definition">¶</a></dt>
<dd><p>Defines the cryptographic capabilities of the key.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyResult.rotation_period">
<code class="descname">rotation_period</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyResult.rotation_period" title="Permalink to this definition">¶</a></dt>
<dd><p>Every time this period passes, generate a new CryptoKeyVersion and set it as
the primary. The first rotation will take place after the specified period. The rotation period has the format
of a decimal number with up to 9 fractional digits, followed by the letter s (seconds).</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyResult.self_link">
<code class="descname">self_link</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyResult.self_link" title="Permalink to this definition">¶</a></dt>
<dd><p>The self link of the created CryptoKey. Its format is <code class="docutils literal notranslate"><span class="pre">projects/{projectId}/locations/{location}/keyRings/{keyRingName}/cryptoKeys/{cryptoKeyName}</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyVersionResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">GetKMSCryptoKeyVersionResult</code><span class="sig-paren">(</span><em>algorithm=None</em>, <em>crypto_key=None</em>, <em>protection_level=None</em>, <em>public_key=None</em>, <em>state=None</em>, <em>version=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyVersionResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getKMSCryptoKeyVersion.</p>
<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.algorithm">
<code class="descname">algorithm</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.algorithm" title="Permalink to this definition">¶</a></dt>
<dd><p>The CryptoKeyVersionAlgorithm that this CryptoKeyVersion supports.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.protection_level">
<code class="descname">protection_level</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.protection_level" title="Permalink to this definition">¶</a></dt>
<dd><p>The ProtectionLevel describing how crypto operations are performed with this CryptoKeyVersion. See the <a class="reference external" href="https://cloud.google.com/kms/docs/reference/rest/v1/ProtectionLevel">protection_level reference</a> for possible outputs.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.public_key">
<code class="descname">public_key</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.public_key" title="Permalink to this definition">¶</a></dt>
<dd><p>If the enclosing CryptoKey has purpose <code class="docutils literal notranslate"><span class="pre">ASYMMETRIC_SIGN</span></code> or <code class="docutils literal notranslate"><span class="pre">ASYMMETRIC_DECRYPT</span></code>, this block contains details about the public key associated to this CryptoKeyVersion. Structure is documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.state">
<code class="descname">state</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.state" title="Permalink to this definition">¶</a></dt>
<dd><p>The current state of the CryptoKeyVersion. See the <a class="reference external" href="https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions#CryptoKeyVersion.CryptoKeyVersionState">state reference</a> for possible outputs.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSCryptoKeyVersionResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.GetKMSKeyRingResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">GetKMSKeyRingResult</code><span class="sig-paren">(</span><em>location=None</em>, <em>name=None</em>, <em>project=None</em>, <em>self_link=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.GetKMSKeyRingResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getKMSKeyRing.</p>
<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSKeyRingResult.self_link">
<code class="descname">self_link</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSKeyRingResult.self_link" title="Permalink to this definition">¶</a></dt>
<dd><p>The self link of the created KeyRing. Its format is <code class="docutils literal notranslate"><span class="pre">projects/{projectId}/locations/{location}/keyRings/{keyRingName}</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSKeyRingResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSKeyRingResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.GetKMSSecretResult">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">GetKMSSecretResult</code><span class="sig-paren">(</span><em>ciphertext=None</em>, <em>crypto_key=None</em>, <em>plaintext=None</em>, <em>id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.GetKMSSecretResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getKMSSecret.</p>
<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSSecretResult.plaintext">
<code class="descname">plaintext</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSSecretResult.plaintext" title="Permalink to this definition">¶</a></dt>
<dd><p>Contains the result of decrypting the provided ciphertext.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.GetKMSSecretResult.id">
<code class="descname">id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.GetKMSSecretResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>id is the provider-assigned unique ID for this managed resource.</p>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.KeyRing">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">KeyRing</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>location=None</em>, <em>name=None</em>, <em>project=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRing" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">KeyRing</span></code> is a toplevel logical grouping of <code class="docutils literal notranslate"><span class="pre">CryptoKeys</span></code>.</p>
<blockquote>
<div><strong>Note:</strong> KeyRings cannot be deleted from Google Cloud Platform.
Destroying a KeyRing will remove it from state but
<em>will not delete the resource on the server.</em></div></blockquote>
<p>To get more information about KeyRing, see:</p>
<ul class="simple">
<li><a class="reference external" href="https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings">API documentation</a></li>
<li>How-to Guides<ul>
<li><a class="reference external" href="https://cloud.google.com/kms/docs/creating-keys#create_a_key_ring">Creating a key ring</a></li>
</ul>
</li>
</ul>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRing.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRing.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.kms.KeyRing.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>location=None</em>, <em>name=None</em>, <em>project=None</em>, <em>self_link=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRing.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing KeyRing resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] project: The ID of the project in which the resource belongs.</p>
<blockquote>
<div>If it is not provided, the provider project is used.</div></blockquote>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRing.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRing.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRing.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRing.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.KeyRingIAMBinding">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">KeyRingIAMBinding</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>key_ring_id=None</em>, <em>members=None</em>, <em>role=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMBinding" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for KMS key ring. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the key ring and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the key ring are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the key ring are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>key_ring_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_binding.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMBinding.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMBinding.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the key ring’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMBinding.key_ring_id">
<code class="descname">key_ring_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMBinding.key_ring_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMBinding.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMBinding.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.kms.KeyRingIAMBinding.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>key_ring_id=None</em>, <em>members=None</em>, <em>role=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMBinding.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing KeyRingIAMBinding resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the key ring’s IAM policy.
:param pulumi.Input[str] key_ring_id: The key ring ID, in the form</p>
<blockquote>
<div><code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_binding.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_binding.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRingIAMBinding.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMBinding.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRingIAMBinding.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMBinding.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.KeyRingIAMMember">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">KeyRingIAMMember</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>key_ring_id=None</em>, <em>member=None</em>, <em>role=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMMember" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for KMS key ring. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the key ring and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the key ring are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the key ring are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>key_ring_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</li>
<li><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_member.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMMember.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMMember.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the key ring’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMMember.key_ring_id">
<code class="descname">key_ring_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMMember.key_ring_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMMember.role">
<code class="descname">role</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMMember.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.kms.KeyRingIAMMember.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>key_ring_id=None</em>, <em>member=None</em>, <em>role=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMMember.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing KeyRingIAMMember resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the key ring’s IAM policy.
:param pulumi.Input[str] key_ring_id: The key ring ID, in the form</p>
<blockquote>
<div><code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role that should be applied. Only one
<code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> can be used per role. Note that custom roles must be of the format
<code class="docutils literal notranslate"><span class="pre">[projects|organizations]/{parent-name}/roles/{role-name}</span></code>.</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_member.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_member.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRingIAMMember.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMMember.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRingIAMMember.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMMember.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.KeyRingIAMPolicy">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">KeyRingIAMPolicy</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>key_ring_id=None</em>, <em>policy_data=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMPolicy" title="Permalink to this definition">¶</a></dt>
<dd><p>Three different resources help you manage your IAM policy for KMS key ring. Each of these resources serves a different use case:</p>
<ul class="simple">
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMPolicy</span></code>: Authoritative. Sets the IAM policy for the key ring and replaces any existing policy already attached.</li>
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code>: Authoritative for a given role. Updates the IAM policy to grant a role to a list of members. Other roles within the IAM policy for the key ring are preserved.</li>
<li><code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code>: Non-authoritative. Updates the IAM policy to grant a role to a new member. Other members for the role for the key ring are preserved.</li>
</ul>
<blockquote>
<div><p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMPolicy</span></code> <strong>cannot</strong> be used in conjunction with <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> and <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code> or they will fight over what your policy should be.</p>
<p><strong>Note:</strong> <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMBinding</span></code> resources <strong>can be</strong> used in conjunction with <code class="docutils literal notranslate"><span class="pre">kms.KeyRingIAMMember</span></code> resources <strong>only if</strong> they do not grant privilege to the same role.</p>
</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>key_ring_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</li>
<li><strong>policy_data</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The policy data generated by
a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_policy.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMPolicy.etag">
<code class="descname">etag</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMPolicy.etag" title="Permalink to this definition">¶</a></dt>
<dd><p>(Computed) The etag of the key ring’s IAM policy.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMPolicy.key_ring_id">
<code class="descname">key_ring_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMPolicy.key_ring_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The key ring ID, in the form
<code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.KeyRingIAMPolicy.policy_data">
<code class="descname">policy_data</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMPolicy.policy_data" title="Permalink to this definition">¶</a></dt>
<dd><p>The policy data generated by
a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.kms.KeyRingIAMPolicy.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>etag=None</em>, <em>key_ring_id=None</em>, <em>policy_data=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMPolicy.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing KeyRingIAMPolicy resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] etag: (Computed) The etag of the key ring’s IAM policy.
:param pulumi.Input[str] key_ring_id: The key ring ID, in the form</p>
<blockquote>
<div><code class="docutils literal notranslate"><span class="pre">{project_id}/{location_name}/{key_ring_name}</span></code> or
<code class="docutils literal notranslate"><span class="pre">{location_name}/{key_ring_name}</span></code>. In the second form, the provider’s
project setting will be used as a fallback.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>policy_data</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The policy data generated by
a <code class="docutils literal notranslate"><span class="pre">organizations.getIAMPolicy</span></code> data source.</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_policy.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/kms_key_ring_iam_policy.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRingIAMPolicy.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMPolicy.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.KeyRingIAMPolicy.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.KeyRingIAMPolicy.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="class">
<dt id="pulumi_gcp.kms.Registry">
<em class="property">class </em><code class="descclassname">pulumi_gcp.kms.</code><code class="descname">Registry</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>credentials=None</em>, <em>event_notification_config=None</em>, <em>http_config=None</em>, <em>mqtt_config=None</em>, <em>name=None</em>, <em>project=None</em>, <em>region=None</em>, <em>state_notification_config=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.Registry" title="Permalink to this definition">¶</a></dt>
<dd><blockquote>
<div>Creates a device registry in Google’s Cloud IoT Core platform. For more information see</div></blockquote>
<p><a class="reference external" href="https://cloud.google.com/iot/docs/">the official documentation</a> and
<a class="reference external" href="https://cloud.google.com/iot/docs/reference/cloudiot/rest/v1/projects.locations.registries">API</a>.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>credentials</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of public key certificates to authenticate devices. Structure is documented below.</li>
<li><strong>event_notification_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A PubSub topics to publish device events. Structure is documented below.</li>
<li><strong>http_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Activate or deactivate HTTP. Structure is documented below.</li>
<li><strong>mqtt_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Activate or deactivate MQTT. Structure is documented below.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A unique name for the resource, required by device registry.
Changing this forces a new resource to be created.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it is not provided, the provider project is used.</li>
<li><strong>region</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Region in which the created address should reside. If it is not provided, the provider region is used.</li>
<li><strong>state_notification_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A PubSub topic to publish device state updates. Structure is documented below.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/cloudiot_registry.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/cloudiot_registry.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.credentials">
<code class="descname">credentials</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.credentials" title="Permalink to this definition">¶</a></dt>
<dd><p>List of public key certificates to authenticate devices. Structure is documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.event_notification_config">
<code class="descname">event_notification_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.event_notification_config" title="Permalink to this definition">¶</a></dt>
<dd><p>A PubSub topics to publish device events. Structure is documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.http_config">
<code class="descname">http_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.http_config" title="Permalink to this definition">¶</a></dt>
<dd><p>Activate or deactivate HTTP. Structure is documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.mqtt_config">
<code class="descname">mqtt_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.mqtt_config" title="Permalink to this definition">¶</a></dt>
<dd><p>Activate or deactivate MQTT. Structure is documented below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.name" title="Permalink to this definition">¶</a></dt>
<dd><p>A unique name for the resource, required by device registry.
Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The project in which the resource belongs. If it is not provided, the provider project is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.region">
<code class="descname">region</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.region" title="Permalink to this definition">¶</a></dt>
<dd><p>The Region in which the created address should reside. If it is not provided, the provider region is used.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.kms.Registry.state_notification_config">
<code class="descname">state_notification_config</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.kms.Registry.state_notification_config" title="Permalink to this definition">¶</a></dt>
<dd><p>A PubSub topic to publish device state updates. Structure is documented below.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_gcp.kms.Registry.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>credentials=None</em>, <em>event_notification_config=None</em>, <em>http_config=None</em>, <em>mqtt_config=None</em>, <em>name=None</em>, <em>project=None</em>, <em>region=None</em>, <em>state_notification_config=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.Registry.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Registry resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[list] credentials: List of public key certificates to authenticate devices. Structure is documented below. 
:param pulumi.Input[dict] event_notification_config: A PubSub topics to publish device events. Structure is documented below.
:param pulumi.Input[dict] http_config: Activate or deactivate HTTP. Structure is documented below.
:param pulumi.Input[dict] mqtt_config: Activate or deactivate MQTT. Structure is documented below.
:param pulumi.Input[str] name: A unique name for the resource, required by device registry.</p>
<blockquote>
<div>Changing this forces a new resource to be created.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The project in which the resource belongs. If it is not provided, the provider project is used.</li>
<li><strong>region</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Region in which the created address should reside. If it is not provided, the provider region is used.</li>
<li><strong>state_notification_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A PubSub topic to publish device state updates. Structure is documented below.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/cloudiot_registry.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/cloudiot_registry.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.Registry.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.Registry.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.kms.Registry.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.Registry.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><strong>prop</strong> (<em>str</em>) – A property name.</td>
</tr>
<tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body">A potentially transformed property name.</td>
</tr>
<tr class="field-odd field"><th class="field-name">Return type:</th><td class="field-body">str</td>
</tr>
</tbody>
</table>
</dd></dl>

</dd></dl>

<dl class="function">
<dt id="pulumi_gcp.kms.get_kms_crypto_key">
<code class="descclassname">pulumi_gcp.kms.</code><code class="descname">get_kms_crypto_key</code><span class="sig-paren">(</span><em>key_ring=None</em>, <em>name=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.get_kms_crypto_key" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides access to a Google Cloud Platform KMS CryptoKey. For more information see
<a class="reference external" href="https://cloud.google.com/kms/docs/object-hierarchy#key">the official documentation</a>
and
<a class="reference external" href="https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys">API</a>.</p>
<p>A CryptoKey is an interface to key material which can be used to encrypt and decrypt data. A CryptoKey belongs to a
Google Cloud KMS KeyRing.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_crypto_key.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_crypto_key.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_gcp.kms.get_kms_crypto_key_version">
<code class="descclassname">pulumi_gcp.kms.</code><code class="descname">get_kms_crypto_key_version</code><span class="sig-paren">(</span><em>crypto_key=None</em>, <em>public_key=None</em>, <em>version=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.get_kms_crypto_key_version" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides access to a Google Cloud Platform KMS CryptoKeyVersion. For more information see
<a class="reference external" href="https://cloud.google.com/kms/docs/object-hierarchy#key_version">the official documentation</a>
and
<a class="reference external" href="https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions">API</a>.</p>
<p>A CryptoKeyVersion represents an individual cryptographic key, and the associated key material.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_crypto_key_version.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_crypto_key_version.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_gcp.kms.get_kms_key_ring">
<code class="descclassname">pulumi_gcp.kms.</code><code class="descname">get_kms_key_ring</code><span class="sig-paren">(</span><em>location=None</em>, <em>name=None</em>, <em>project=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.get_kms_key_ring" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides access to Google Cloud Platform KMS KeyRing. For more information see
<a class="reference external" href="https://cloud.google.com/kms/docs/object-hierarchy#key_ring">the official documentation</a>
and
<a class="reference external" href="https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings">API</a>.</p>
<p>A KeyRing is a grouping of CryptoKeys for organizational purposes. A KeyRing belongs to a Google Cloud Platform Project
and resides in a specific location.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_key_ring.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_key_ring.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="function">
<dt id="pulumi_gcp.kms.get_kms_secret">
<code class="descclassname">pulumi_gcp.kms.</code><code class="descname">get_kms_secret</code><span class="sig-paren">(</span><em>ciphertext=None</em>, <em>crypto_key=None</em>, <em>opts=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.kms.get_kms_secret" title="Permalink to this definition">¶</a></dt>
<dd><p>This data source allows you to use data encrypted with Google Cloud KMS
within your resource definitions.</p>
<p>For more information see
<a class="reference external" href="https://cloud.google.com/kms/docs/encrypt-decrypt">the official documentation</a>.</p>
<blockquote>
<div><p><strong>NOTE</strong>: Using this data provider will allow you to conceal secret data within your
resource definitions, but it does not take care of protecting that data in the
logging output, plan output, or state output.  Please take care to secure your secret
data outside of resource definitions.</p>
<p>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_secret.html.markdown">https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/d/kms_secret.html.markdown</a>.</p>
</div></blockquote>
</dd></dl>

</div>
