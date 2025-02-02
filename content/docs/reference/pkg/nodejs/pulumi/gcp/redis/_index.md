---
title: Module redis
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/gcp</a> &gt; redis

> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-google)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-gcp` repo](https://github.com/pulumi/pulumi-gcp/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-google` repo](https://github.com/terraform-providers/terraform-provider-google/issues).



<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Instance">class Instance</a></li>
<li><a href="#InstanceArgs">interface InstanceArgs</a></li>
<li><a href="#InstanceState">interface InstanceState</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts">redis/instance.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Instance">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L54">class <b>Instance</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

A Google Cloud Redis instance.

To get more information about Instance, see:

* [API documentation](https://cloud.google.com/memorystore/docs/redis/reference/rest/)
* How-to Guides
    * [Official Documentation](https://cloud.google.com/memorystore/docs/redis/)

## Example Usage - Redis Instance Basic


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as gcp from "@pulumi/gcp";

const cache = new gcp.redis.Instance("cache", {
    memorySizeGb: 1,
});
```
## Example Usage - Redis Instance Full


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as gcp from "@pulumi/gcp";

const autoNetwork = new gcp.compute.Network("auto-network", {});
const cache = new gcp.redis.Instance("cache", {
    alternativeLocationId: "us-central1-f",
    authorizedNetwork: auto_network.selfLink,
    displayName: "Test Instance",
    labels: {
        my_key: "myVal",
        other_key: "otherVal",
    },
    locationId: "us-central1-a",
    memorySizeGb: 1,
    redisVersion: "REDIS_3_2",
    reservedIpRange: "192.168.0.0/29",
    tier: "STANDARD_HA",
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/redis_instance.html.markdown.

{{% /md %}}
<h3 class="pdoc-member-header" id="Instance-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L101"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Instance(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#InstanceArgs'>InstanceArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Instance resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L63">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#InstanceState'>InstanceState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Instance'>Instance</a></pre>


Get an existing Instance resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L74">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of Instance.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-alternativeLocationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L81">property <b>alternativeLocationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>alternativeLocationId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-authorizedNetwork">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L82">property <b>authorizedNetwork</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>authorizedNetwork: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-createTime">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L83">property <b>createTime</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>createTime: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-currentLocationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L84">property <b>currentLocationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>currentLocationId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L85">property <b>displayName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>displayName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-host">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L86">property <b>host</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>host: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L212">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-labels">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L87">property <b>labels</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>labels: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-locationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L88">property <b>locationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>locationId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-memorySizeGb">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L89">property <b>memorySizeGb</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>memorySizeGb: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L90">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-port">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L91">property <b>port</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>port: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L96">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>project: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-redisConfigs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L97">property <b>redisConfigs</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>redisConfigs: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-redisVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L98">property <b>redisVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>redisVersion: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-region">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L99">property <b>region</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>region: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-reservedIpRange">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L100">property <b>reservedIpRange</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>reservedIpRange: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-tier">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L101">property <b>tier</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>tier: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Instance-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="InstanceArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L196">interface <b>InstanceArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a Instance resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="InstanceArgs-alternativeLocationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L197">property <b>alternativeLocationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>alternativeLocationId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-authorizedNetwork">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L198">property <b>authorizedNetwork</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>authorizedNetwork?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L199">property <b>displayName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>displayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-labels">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L200">property <b>labels</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>labels?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-locationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L201">property <b>locationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>locationId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-memorySizeGb">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L202">property <b>memorySizeGb</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>memorySizeGb: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L203">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L208">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>project?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-redisConfigs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L209">property <b>redisConfigs</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>redisConfigs?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-redisVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L210">property <b>redisVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>redisVersion?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-region">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L211">property <b>region</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>region?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-reservedIpRange">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L212">property <b>reservedIpRange</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>reservedIpRange?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceArgs-tier">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L213">property <b>tier</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>tier?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="InstanceState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L169">interface <b>InstanceState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering Instance resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="InstanceState-alternativeLocationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L170">property <b>alternativeLocationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>alternativeLocationId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-authorizedNetwork">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L171">property <b>authorizedNetwork</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>authorizedNetwork?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-createTime">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L172">property <b>createTime</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>createTime?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-currentLocationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L173">property <b>currentLocationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>currentLocationId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L174">property <b>displayName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>displayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-host">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L175">property <b>host</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>host?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-labels">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L176">property <b>labels</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>labels?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-locationId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L177">property <b>locationId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>locationId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-memorySizeGb">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L178">property <b>memorySizeGb</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>memorySizeGb?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L179">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-port">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L180">property <b>port</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>port?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L185">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>project?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-redisConfigs">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L186">property <b>redisConfigs</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>redisConfigs?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-redisVersion">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L187">property <b>redisVersion</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>redisVersion?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-region">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L188">property <b>region</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>region?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-reservedIpRange">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L189">property <b>reservedIpRange</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>reservedIpRange?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="InstanceState-tier">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/e0c4a091bee188617832b38acaf43fc66101bbac/sdk/nodejs/redis/instance.ts#L190">property <b>tier</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>tier?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}
{{% /md %}}
</div>
</div>
