---
title: Module mediaservices
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/azure</a> &gt; mediaservices

> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-azurerm)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-azure` repo](https://github.com/pulumi/pulumi-azure/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-azurerm` repo](https://github.com/terraform-providers/terraform-provider-azurerm/issues).



<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Account">class Account</a></li>
<li><a href="#AccountArgs">interface AccountArgs</a></li>
<li><a href="#AccountState">interface AccountState</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts">mediaservices/account.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Account">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L40">class <b>Account</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

Manages a Media Services Account.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure from "@pulumi/azure";

const testResourceGroup = new azure.core.ResourceGroup("test", {
    location: "West Europe",
    name: "media-resources",
});
const testStorageAccount = new azure.storage.Account("test", {
    accountReplicationType: "GRS",
    accountTier: "Standard",
    location: testResourceGroup.location,
    name: "examplestoracc",
    resourceGroupName: testResourceGroup.name,
});
const testAccount = new azure.mediaservices.Account("test", {
    location: testResourceGroup.location,
    name: "examplemediaacc",
    resourceGroupName: testResourceGroup.name,
    storageAccounts: [{
        id: testStorageAccount.id,
        isPrimary: true,
    }],
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/media_services_account.html.markdown.

{{% /md %}}
<h3 class="pdoc-member-header" id="Account-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L82"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Account(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#AccountArgs'>AccountArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Account resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L49">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#AccountState'>AccountState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Account'>Account</a></pre>


Get an existing Account resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L60">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of Account.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L212">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L70">property <b>location</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>location: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L74">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Specifies the name of the Media Services Account. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-resourceGroupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L78">property <b>resourceGroupName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>resourceGroupName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The name of the resource group in which to create the Media Services Account. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-storageAccounts">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L82">property <b>storageAccounts</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>storageAccounts: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{
    id: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    isPrimary: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'>false</span> | <span class='kd'>true</span>;
}[]&gt;;</pre>
{{% md %}}

One or more `storageAccount` blocks as defined below.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Account-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="AccountArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L149">interface <b>AccountArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a Account resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="AccountArgs-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L153">property <b>location</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>location?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="AccountArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L157">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Specifies the name of the Media Services Account. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="AccountArgs-resourceGroupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L161">property <b>resourceGroupName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>resourceGroupName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The name of the resource group in which to create the Media Services Account. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="AccountArgs-storageAccounts">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L165">property <b>storageAccounts</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>storageAccounts: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    isPrimary: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;
}&gt;[]&gt;;</pre>
{{% md %}}

One or more `storageAccount` blocks as defined below.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="AccountState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L127">interface <b>AccountState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering Account resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="AccountState-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L131">property <b>location</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>location?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="AccountState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L135">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Specifies the name of the Media Services Account. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="AccountState-resourceGroupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L139">property <b>resourceGroupName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>resourceGroupName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The name of the resource group in which to create the Media Services Account. Changing this forces a new resource to be created.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="AccountState-storageAccounts">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/c65ecc4d5fd47a6b7a09d5ea6a52c7a6c272d648/sdk/nodejs/mediaservices/account.ts#L143">property <b>storageAccounts</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>storageAccounts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    isPrimary: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;
}&gt;[]&gt;;</pre>
{{% md %}}

One or more `storageAccount` blocks as defined below.

{{% /md %}}
</div>
</div>
