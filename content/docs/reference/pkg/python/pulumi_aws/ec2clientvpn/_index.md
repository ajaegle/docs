---
title: Module ec2clientvpn
---

<div class="section" id="ec2clientvpn">
<h1>ec2clientvpn<a class="headerlink" href="#ec2clientvpn" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-aws/issues">pulumi/pulumi-aws repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/issues">terraform-providers/terraform-provider-aws repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_aws.ec2clientvpn"></span><dl class="class">
<dt id="pulumi_aws.ec2clientvpn.Endpoint">
<em class="property">class </em><code class="descclassname">pulumi_aws.ec2clientvpn.</code><code class="descname">Endpoint</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>authentication_options=None</em>, <em>client_cidr_block=None</em>, <em>connection_log_options=None</em>, <em>description=None</em>, <em>dns_servers=None</em>, <em>server_certificate_arn=None</em>, <em>split_tunnel=None</em>, <em>tags=None</em>, <em>transport_protocol=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides an AWS Client VPN endpoint for OpenVPN clients. For more information on usage, please see the
<a class="reference external" href="https://docs.aws.amazon.com/vpn/latest/clientvpn-admin/what-is.html">AWS Client VPN Administrator’s Guide</a>.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>authentication_options</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Information about the authentication method to be used to authenticate clients.</li>
<li><strong>client_cidr_block</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The IPv4 address range, in CIDR notation, from which to assign client IP addresses. The address range cannot overlap with the local CIDR of the VPC in which the associated subnet is located, or the routes that you add manually. The address range cannot be changed after the Client VPN endpoint has been created. The CIDR block should be /22 or greater.</li>
<li><strong>connection_log_options</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Information about the client connection logging options.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Name of the repository.</li>
<li><strong>dns_servers</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – Information about the DNS servers to be used for DNS resolution. A Client VPN endpoint can have up to two DNS servers. If no DNS server is specified, the DNS address of the VPC that is to be associated with Client VPN endpoint is used as the DNS server.</li>
<li><strong>server_certificate_arn</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ARN of the ACM server certificate.</li>
<li><strong>split_tunnel</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Indicates whether split-tunnel is enabled on VPN endpoint. Default value is <code class="docutils literal notranslate"><span class="pre">false</span></code>.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>transport_protocol</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The transport protocol to be used by the VPN session. Default value is <code class="docutils literal notranslate"><span class="pre">udp</span></code>.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_endpoint.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_endpoint.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.authentication_options">
<code class="descname">authentication_options</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.authentication_options" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the authentication method to be used to authenticate clients.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.client_cidr_block">
<code class="descname">client_cidr_block</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.client_cidr_block" title="Permalink to this definition">¶</a></dt>
<dd><p>The IPv4 address range, in CIDR notation, from which to assign client IP addresses. The address range cannot overlap with the local CIDR of the VPC in which the associated subnet is located, or the routes that you add manually. The address range cannot be changed after the Client VPN endpoint has been created. The CIDR block should be /22 or greater.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.connection_log_options">
<code class="descname">connection_log_options</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.connection_log_options" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the client connection logging options.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.description" title="Permalink to this definition">¶</a></dt>
<dd><p>Name of the repository.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.dns_name">
<code class="descname">dns_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.dns_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The DNS name to be used by clients when establishing their VPN session.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.dns_servers">
<code class="descname">dns_servers</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.dns_servers" title="Permalink to this definition">¶</a></dt>
<dd><p>Information about the DNS servers to be used for DNS resolution. A Client VPN endpoint can have up to two DNS servers. If no DNS server is specified, the DNS address of the VPC that is to be associated with Client VPN endpoint is used as the DNS server.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.server_certificate_arn">
<code class="descname">server_certificate_arn</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.server_certificate_arn" title="Permalink to this definition">¶</a></dt>
<dd><p>The ARN of the ACM server certificate.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.split_tunnel">
<code class="descname">split_tunnel</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.split_tunnel" title="Permalink to this definition">¶</a></dt>
<dd><p>Indicates whether split-tunnel is enabled on VPN endpoint. Default value is <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.status">
<code class="descname">status</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.status" title="Permalink to this definition">¶</a></dt>
<dd><p>The current state of the Client VPN endpoint.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.transport_protocol">
<code class="descname">transport_protocol</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.transport_protocol" title="Permalink to this definition">¶</a></dt>
<dd><p>The transport protocol to be used by the VPN session. Default value is <code class="docutils literal notranslate"><span class="pre">udp</span></code>.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>authentication_options=None</em>, <em>client_cidr_block=None</em>, <em>connection_log_options=None</em>, <em>description=None</em>, <em>dns_name=None</em>, <em>dns_servers=None</em>, <em>server_certificate_arn=None</em>, <em>split_tunnel=None</em>, <em>status=None</em>, <em>tags=None</em>, <em>transport_protocol=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Endpoint resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] authentication_options: Information about the authentication method to be used to authenticate clients.
:param pulumi.Input[str] client_cidr_block: The IPv4 address range, in CIDR notation, from which to assign client IP addresses. The address range cannot overlap with the local CIDR of the VPC in which the associated subnet is located, or the routes that you add manually. The address range cannot be changed after the Client VPN endpoint has been created. The CIDR block should be /22 or greater.
:param pulumi.Input[dict] connection_log_options: Information about the client connection logging options.
:param pulumi.Input[str] description: Name of the repository.
:param pulumi.Input[str] dns_name: The DNS name to be used by clients when establishing their VPN session.
:param pulumi.Input[list] dns_servers: Information about the DNS servers to be used for DNS resolution. A Client VPN endpoint can have up to two DNS servers. If no DNS server is specified, the DNS address of the VPC that is to be associated with Client VPN endpoint is used as the DNS server.
:param pulumi.Input[str] server_certificate_arn: The ARN of the ACM server certificate.
:param pulumi.Input[bool] split_tunnel: Indicates whether split-tunnel is enabled on VPN endpoint. Default value is <code class="docutils literal notranslate"><span class="pre">false</span></code>.
:param pulumi.Input[str] status: The current state of the Client VPN endpoint.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[str] transport_protocol: The transport protocol to be used by the VPN session. Default value is <code class="docutils literal notranslate"><span class="pre">udp</span></code>.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_endpoint.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_endpoint.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_aws.ec2clientvpn.Endpoint.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.ec2clientvpn.Endpoint.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.Endpoint.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation">
<em class="property">class </em><code class="descclassname">pulumi_aws.ec2clientvpn.</code><code class="descname">NetworkAssociation</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>client_vpn_endpoint_id=None</em>, <em>subnet_id=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides network associations for AWS Client VPN endpoints. For more information on usage, please see the 
<a class="reference external" href="https://docs.aws.amazon.com/vpn/latest/clientvpn-admin/what-is.html">AWS Client VPN Administrator’s Guide</a>.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>client_vpn_endpoint_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the Client VPN endpoint.</li>
<li><strong>subnet_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the subnet to associate with the Client VPN endpoint.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_network_association.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_network_association.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.client_vpn_endpoint_id">
<code class="descname">client_vpn_endpoint_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.client_vpn_endpoint_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the Client VPN endpoint.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.security_groups">
<code class="descname">security_groups</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.security_groups" title="Permalink to this definition">¶</a></dt>
<dd><p>The IDs of the security groups applied to the target network association.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.status">
<code class="descname">status</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.status" title="Permalink to this definition">¶</a></dt>
<dd><p>The current state of the target network association.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.subnet_id">
<code class="descname">subnet_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.subnet_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the subnet to associate with the Client VPN endpoint.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.vpc_id">
<code class="descname">vpc_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.vpc_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the VPC in which the target network (subnet) is located.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>client_vpn_endpoint_id=None</em>, <em>security_groups=None</em>, <em>status=None</em>, <em>subnet_id=None</em>, <em>vpc_id=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing NetworkAssociation resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[str] client_vpn_endpoint_id: The ID of the Client VPN endpoint.
:param pulumi.Input[list] security_groups: The IDs of the security groups applied to the target network association.
:param pulumi.Input[str] status: The current state of the target network association.
:param pulumi.Input[str] subnet_id: The ID of the subnet to associate with the Client VPN endpoint.
:param pulumi.Input[str] vpc_id: The ID of the VPC in which the target network (subnet) is located.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_network_association.html.markdown">https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/ec2_client_vpn_network_association.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_aws.ec2clientvpn.NetworkAssociation.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_aws.ec2clientvpn.NetworkAssociation.translate_input_property" title="Permalink to this definition">¶</a></dt>
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

</div>
