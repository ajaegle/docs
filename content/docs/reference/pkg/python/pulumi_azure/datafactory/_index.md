---
title: Module datafactory
---

<div class="section" id="datafactory">
<h1>datafactory<a class="headerlink" href="#datafactory" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-azure/issues">pulumi/pulumi-azure repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/issues">terraform-providers/terraform-provider-azurerm repo</a>.</div></blockquote>
<span class="target" id="module-pulumi_azure.datafactory"></span><dl class="class">
<dt id="pulumi_azure.datafactory.DatasetMysql">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">DatasetMysql</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>folder=None</em>, <em>linked_service_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>schema_columns=None</em>, <em>table_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a MySQL Dataset inside a Azure Data Factory.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>additional_properties</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of additional properties to associate with the Data Factory Dataset MySQL.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Dataset MySQL.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Dataset MySQL.</li>
<li><strong>folder</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.</li>
<li><strong>linked_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory Linked Service name in which to associate the Dataset with.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the name of the Data Factory Dataset MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Dataset MySQL.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Dataset MySQL. Changing this forces a new resource</li>
<li><strong>schema_columns</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.</li>
<li><strong>table_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The table name of the Data Factory Dataset MySQL.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_mysql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_mysql.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.additional_properties">
<code class="descname">additional_properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.additional_properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of additional properties to associate with the Data Factory Dataset MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Dataset MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Dataset MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.folder">
<code class="descname">folder</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.folder" title="Permalink to this definition">¶</a></dt>
<dd><p>The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.linked_service_name">
<code class="descname">linked_service_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.linked_service_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory Linked Service name in which to associate the Dataset with.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Dataset MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Dataset MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Dataset MySQL. Changing this forces a new resource</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.schema_columns">
<code class="descname">schema_columns</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.schema_columns" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetMysql.table_name">
<code class="descname">table_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.table_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The table name of the Data Factory Dataset MySQL.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.DatasetMysql.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>folder=None</em>, <em>linked_service_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>schema_columns=None</em>, <em>table_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing DatasetMysql resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] additional_properties: A map of additional properties to associate with the Data Factory Dataset MySQL.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Dataset MySQL.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Dataset MySQL.
:param pulumi.Input[str] folder: The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.
:param pulumi.Input[str] linked_service_name: The Data Factory Linked Service name in which to associate the Dataset with.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Dataset MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Dataset MySQL.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Dataset MySQL. Changing this forces a new resource
:param pulumi.Input[list] schema_columns: A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.
:param pulumi.Input[str] table_name: The table name of the Data Factory Dataset MySQL.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_mysql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_mysql.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.DatasetMysql.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.DatasetMysql.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetMysql.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.DatasetPostgresql">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">DatasetPostgresql</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>folder=None</em>, <em>linked_service_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>schema_columns=None</em>, <em>table_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a PostgreSQL Dataset inside a Azure Data Factory.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>additional_properties</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of additional properties to associate with the Data Factory Dataset PostgreSQL.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Dataset PostgreSQL.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Dataset PostgreSQL.</li>
<li><strong>folder</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.</li>
<li><strong>linked_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory Linked Service name in which to associate the Dataset with.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory Dataset PostgreSQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Dataset PostgreSQL.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Dataset PostgreSQL. Changing this forces a new resource</li>
<li><strong>schema_columns</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.</li>
<li><strong>table_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The table name of the Data Factory Dataset PostgreSQL.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_postgresql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_postgresql.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.additional_properties">
<code class="descname">additional_properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.additional_properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of additional properties to associate with the Data Factory Dataset PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Dataset PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Dataset PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.folder">
<code class="descname">folder</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.folder" title="Permalink to this definition">¶</a></dt>
<dd><p>The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.linked_service_name">
<code class="descname">linked_service_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.linked_service_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory Linked Service name in which to associate the Dataset with.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Dataset PostgreSQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Dataset PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Dataset PostgreSQL. Changing this forces a new resource</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.schema_columns">
<code class="descname">schema_columns</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.schema_columns" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.table_name">
<code class="descname">table_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.table_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The table name of the Data Factory Dataset PostgreSQL.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>folder=None</em>, <em>linked_service_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>schema_columns=None</em>, <em>table_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing DatasetPostgresql resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] additional_properties: A map of additional properties to associate with the Data Factory Dataset PostgreSQL.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Dataset PostgreSQL.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Dataset PostgreSQL.
:param pulumi.Input[str] folder: The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.
:param pulumi.Input[str] linked_service_name: The Data Factory Linked Service name in which to associate the Dataset with.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Dataset PostgreSQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Dataset PostgreSQL.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Dataset PostgreSQL. Changing this forces a new resource
:param pulumi.Input[list] schema_columns: A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.
:param pulumi.Input[str] table_name: The table name of the Data Factory Dataset PostgreSQL.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_postgresql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_postgresql.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.DatasetPostgresql.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.DatasetPostgresql.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetPostgresql.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">DatasetSqlServerTable</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>folder=None</em>, <em>linked_service_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>schema_columns=None</em>, <em>table_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a SQL Server Table Dataset inside a Azure Data Factory.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>additional_properties</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of additional properties to associate with the Data Factory Dataset SQL Server Table.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Dataset SQL Server Table.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Dataset SQL Server Table.</li>
<li><strong>folder</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.</li>
<li><strong>linked_service_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory Linked Service name in which to associate the Dataset with.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory Dataset SQL Server Table. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Dataset SQL Server Table.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Dataset SQL Server Table. Changing this forces a new resource</li>
<li><strong>schema_columns</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.</li>
<li><strong>table_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The table name of the Data Factory Dataset SQL Server Table.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_sql_server_table.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_sql_server_table.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.additional_properties">
<code class="descname">additional_properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.additional_properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of additional properties to associate with the Data Factory Dataset SQL Server Table.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Dataset SQL Server Table.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Dataset SQL Server Table.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.folder">
<code class="descname">folder</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.folder" title="Permalink to this definition">¶</a></dt>
<dd><p>The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.linked_service_name">
<code class="descname">linked_service_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.linked_service_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory Linked Service name in which to associate the Dataset with.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Dataset SQL Server Table. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Dataset SQL Server Table.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Dataset SQL Server Table. Changing this forces a new resource</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.schema_columns">
<code class="descname">schema_columns</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.schema_columns" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.table_name">
<code class="descname">table_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.table_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The table name of the Data Factory Dataset SQL Server Table.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>folder=None</em>, <em>linked_service_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>schema_columns=None</em>, <em>table_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing DatasetSqlServerTable resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] additional_properties: A map of additional properties to associate with the Data Factory Dataset SQL Server Table.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Dataset SQL Server Table.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Dataset with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Dataset SQL Server Table.
:param pulumi.Input[str] folder: The folder that this Dataset is in. If not specified, the Dataset will appear at the root level.
:param pulumi.Input[str] linked_service_name: The Data Factory Linked Service name in which to associate the Dataset with.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Dataset SQL Server Table. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Dataset SQL Server Table.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Dataset SQL Server Table. Changing this forces a new resource
:param pulumi.Input[list] schema_columns: A <code class="docutils literal notranslate"><span class="pre">schema_column</span></code> block as defined below.
:param pulumi.Input[str] table_name: The table name of the Data Factory Dataset SQL Server Table.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_sql_server_table.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_dataset_sql_server_table.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.DatasetSqlServerTable.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.DatasetSqlServerTable.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.Factory">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">Factory</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>github_configuration=None</em>, <em>identity=None</em>, <em>location=None</em>, <em>name=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>vsts_configuration=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Factory" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage an Azure Data Factory (Version 2).</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>github_configuration</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">github_configuration</span></code> block as defined below.</li>
<li><strong>identity</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – An <code class="docutils literal notranslate"><span class="pre">identity</span></code> block as defined below.</li>
<li><strong>location</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory.</li>
<li><strong>tags</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A mapping of tags to assign to the resource.</li>
<li><strong>vsts_configuration</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A <code class="docutils literal notranslate"><span class="pre">vsts_configuration</span></code> block as defined below.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.Factory.github_configuration">
<code class="descname">github_configuration</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Factory.github_configuration" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">github_configuration</span></code> block as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Factory.identity">
<code class="descname">identity</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Factory.identity" title="Permalink to this definition">¶</a></dt>
<dd><p>An <code class="docutils literal notranslate"><span class="pre">identity</span></code> block as defined below.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Factory.location">
<code class="descname">location</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Factory.location" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Factory.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Factory.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Factory.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Factory.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Factory.tags">
<code class="descname">tags</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Factory.tags" title="Permalink to this definition">¶</a></dt>
<dd><p>A mapping of tags to assign to the resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Factory.vsts_configuration">
<code class="descname">vsts_configuration</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Factory.vsts_configuration" title="Permalink to this definition">¶</a></dt>
<dd><p>A <code class="docutils literal notranslate"><span class="pre">vsts_configuration</span></code> block as defined below.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.Factory.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>github_configuration=None</em>, <em>identity=None</em>, <em>location=None</em>, <em>name=None</em>, <em>resource_group_name=None</em>, <em>tags=None</em>, <em>vsts_configuration=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Factory.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Factory resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] github_configuration: A <code class="docutils literal notranslate"><span class="pre">github_configuration</span></code> block as defined below.
:param pulumi.Input[dict] identity: An <code class="docutils literal notranslate"><span class="pre">identity</span></code> block as defined below.
:param pulumi.Input[str] location: Specifies the supported Azure location where the resource exists. Changing this forces a new resource to be created.
:param pulumi.Input[str] name: Specifies the name of the Data Factory. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory.
:param pulumi.Input[dict] tags: A mapping of tags to assign to the resource.
:param pulumi.Input[dict] vsts_configuration: A <code class="docutils literal notranslate"><span class="pre">vsts_configuration</span></code> block as defined below.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.Factory.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Factory.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.Factory.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Factory.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">LinkedServiceDataLakeStorageGen2</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>service_principal_id=None</em>, <em>service_principal_key=None</em>, <em>tenant=None</em>, <em>url=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a Linked Service (connection) between Data Lake Storage Gen2 and Azure Data Factory.</p>
<blockquote>
<div><strong>Note:</strong> All arguments including the <code class="docutils literal notranslate"><span class="pre">service_principal_key</span></code> will be stored in the raw state as plain-text. <a class="reference external" href="https://www.terraform.io/docs/state/sensitive-data.html">Read more about sensitive data in state</a>.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>additional_properties</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of additional properties to associate with the Data Factory Linked Service MySQL.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Linked Service MySQL.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Linked Service MySQL.</li>
<li><strong>integration_runtime_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The integration runtime reference to associate with the Data Factory Linked Service MySQL.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory Linked Service MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Linked Service MySQL.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Linked Service MySQL. Changing this forces a new resource</li>
<li><strong>service_principal_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The service principal id in which to authenticate against the Azure Data Lake Storage Gen2 account.</li>
<li><strong>service_principal_key</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The service principal key in which to authenticate against the Azure Data Lake Storage Gen2 account.</li>
<li><strong>tenant</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The tenant id or name in which to authenticate against the Azure Data Lake Storage Gen2 account.</li>
<li><strong>url</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The endpoint for the Azure Data Lake Storage Gen2 service.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_data_lake_storage_gen2.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_data_lake_storage_gen2.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.additional_properties">
<code class="descname">additional_properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.additional_properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of additional properties to associate with the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.integration_runtime_name">
<code class="descname">integration_runtime_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.integration_runtime_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The integration runtime reference to associate with the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Linked Service MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Linked Service MySQL. Changing this forces a new resource</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.service_principal_id">
<code class="descname">service_principal_id</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.service_principal_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The service principal id in which to authenticate against the Azure Data Lake Storage Gen2 account.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.service_principal_key">
<code class="descname">service_principal_key</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.service_principal_key" title="Permalink to this definition">¶</a></dt>
<dd><p>The service principal key in which to authenticate against the Azure Data Lake Storage Gen2 account.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.tenant">
<code class="descname">tenant</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.tenant" title="Permalink to this definition">¶</a></dt>
<dd><p>The tenant id or name in which to authenticate against the Azure Data Lake Storage Gen2 account.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.url">
<code class="descname">url</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.url" title="Permalink to this definition">¶</a></dt>
<dd><p>The endpoint for the Azure Data Lake Storage Gen2 service.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>service_principal_id=None</em>, <em>service_principal_key=None</em>, <em>tenant=None</em>, <em>url=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing LinkedServiceDataLakeStorageGen2 resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] additional_properties: A map of additional properties to associate with the Data Factory Linked Service MySQL.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Linked Service MySQL.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Linked Service MySQL.
:param pulumi.Input[str] integration_runtime_name: The integration runtime reference to associate with the Data Factory Linked Service MySQL.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Linked Service MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Linked Service MySQL.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Linked Service MySQL. Changing this forces a new resource
:param pulumi.Input[str] service_principal_id: The service principal id in which to authenticate against the Azure Data Lake Storage Gen2 account.
:param pulumi.Input[str] service_principal_key: The service principal key in which to authenticate against the Azure Data Lake Storage Gen2 account.
:param pulumi.Input[str] tenant: The tenant id or name in which to authenticate against the Azure Data Lake Storage Gen2 account.
:param pulumi.Input[str] url: The endpoint for the Azure Data Lake Storage Gen2 service.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_data_lake_storage_gen2.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_data_lake_storage_gen2.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceDataLakeStorageGen2.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServiceMysql">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">LinkedServiceMysql</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>connection_string=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a Linked Service (connection) between MySQL and Azure Data Factory.</p>
<blockquote>
<div><strong>Note:</strong> All arguments including the connection_string will be stored in the raw state as plain-text. <a class="reference external" href="https://www.terraform.io/docs/state/sensitive-data.html">Read more about sensitive data in state</a>.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>additional_properties</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of additional properties to associate with the Data Factory Linked Service MySQL.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Linked Service MySQL.</li>
<li><strong>connection_string</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The connection string in which to authenticate with MySQL.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Linked Service MySQL.</li>
<li><strong>integration_runtime_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The integration runtime reference to associate with the Data Factory Linked Service MySQL.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory Linked Service MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Linked Service MySQL.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Linked Service MySQL. Changing this forces a new resource</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_mysql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_mysql.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.additional_properties">
<code class="descname">additional_properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.additional_properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of additional properties to associate with the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.connection_string">
<code class="descname">connection_string</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.connection_string" title="Permalink to this definition">¶</a></dt>
<dd><p>The connection string in which to authenticate with MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.integration_runtime_name">
<code class="descname">integration_runtime_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.integration_runtime_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The integration runtime reference to associate with the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Linked Service MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Linked Service MySQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Linked Service MySQL. Changing this forces a new resource</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>connection_string=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing LinkedServiceMysql resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] additional_properties: A map of additional properties to associate with the Data Factory Linked Service MySQL.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Linked Service MySQL.
:param pulumi.Input[str] connection_string: The connection string in which to authenticate with MySQL.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Linked Service MySQL.
:param pulumi.Input[str] integration_runtime_name: The integration runtime reference to associate with the Data Factory Linked Service MySQL.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Linked Service MySQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Linked Service MySQL.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Linked Service MySQL. Changing this forces a new resource</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_mysql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_mysql.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServiceMysql.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceMysql.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">LinkedServicePostgresql</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>connection_string=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a Linked Service (connection) between PostgreSQL and Azure Data Factory.</p>
<blockquote>
<div><strong>Note:</strong> All arguments including the connection_string will be stored in the raw state as plain-text. <a class="reference external" href="https://www.terraform.io/docs/state/sensitive-data.html">Read more about sensitive data in state</a>.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>additional_properties</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of additional properties to associate with the Data Factory Linked Service PostgreSQL.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Linked Service PostgreSQL.</li>
<li><strong>connection_string</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The connection string in which to authenticate with PostgreSQL.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Linked Service PostgreSQL.</li>
<li><strong>integration_runtime_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The integration runtime reference to associate with the Data Factory Linked Service PostgreSQL.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory Linked Service PostgreSQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Linked Service PostgreSQL.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Linked Service PostgreSQL. Changing this forces a new resource</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_postgresql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_postgresql.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.additional_properties">
<code class="descname">additional_properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.additional_properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of additional properties to associate with the Data Factory Linked Service PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Linked Service PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.connection_string">
<code class="descname">connection_string</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.connection_string" title="Permalink to this definition">¶</a></dt>
<dd><p>The connection string in which to authenticate with PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Linked Service PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.integration_runtime_name">
<code class="descname">integration_runtime_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.integration_runtime_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The integration runtime reference to associate with the Data Factory Linked Service PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Linked Service PostgreSQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Linked Service PostgreSQL.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Linked Service PostgreSQL. Changing this forces a new resource</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>connection_string=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing LinkedServicePostgresql resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] additional_properties: A map of additional properties to associate with the Data Factory Linked Service PostgreSQL.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Linked Service PostgreSQL.
:param pulumi.Input[str] connection_string: The connection string in which to authenticate with PostgreSQL.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Linked Service PostgreSQL.
:param pulumi.Input[str] integration_runtime_name: The integration runtime reference to associate with the Data Factory Linked Service PostgreSQL.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Linked Service PostgreSQL. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Linked Service PostgreSQL.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Linked Service PostgreSQL. Changing this forces a new resource</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_postgresql.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_postgresql.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServicePostgresql.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServicePostgresql.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">LinkedServiceSqlServer</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>connection_string=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a Linked Service (connection) between a SQL Server and Azure Data Factory.</p>
<blockquote>
<div><strong>Note:</strong> All arguments including the client secret will be stored in the raw state as plain-text. <a class="reference external" href="https://www.terraform.io/docs/state/sensitive-data.html">Read more about sensitive data in state</a>.</div></blockquote>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>additional_properties</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of additional properties to associate with the Data Factory Linked Service SQL Server.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Linked Service SQL Server.</li>
<li><strong>connection_string</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The connection string in which to authenticate with the SQL Server.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Linked Service SQL Server.</li>
<li><strong>integration_runtime_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The integration runtime reference to associate with the Data Factory Linked Service SQL Server.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory Linked Service SQL Server. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Linked Service SQL Server.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Linked Service SQL Server. Changing this forces a new resource</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_sql_server.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_sql_server.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.additional_properties">
<code class="descname">additional_properties</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.additional_properties" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of additional properties to associate with the Data Factory Linked Service SQL Server.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Linked Service SQL Server.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.connection_string">
<code class="descname">connection_string</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.connection_string" title="Permalink to this definition">¶</a></dt>
<dd><p>The connection string in which to authenticate with the SQL Server.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Linked Service SQL Server.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.integration_runtime_name">
<code class="descname">integration_runtime_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.integration_runtime_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The integration runtime reference to associate with the Data Factory Linked Service SQL Server.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Linked Service SQL Server. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Linked Service SQL Server.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Linked Service SQL Server. Changing this forces a new resource</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>additional_properties=None</em>, <em>annotations=None</em>, <em>connection_string=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>integration_runtime_name=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing LinkedServiceSqlServer resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[dict] additional_properties: A map of additional properties to associate with the Data Factory Linked Service SQL Server.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Linked Service SQL Server.
:param pulumi.Input[str] connection_string: The connection string in which to authenticate with the SQL Server.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Linked Service with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Linked Service SQL Server.
:param pulumi.Input[str] integration_runtime_name: The integration runtime reference to associate with the Data Factory Linked Service SQL Server.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Linked Service SQL Server. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Linked Service SQL Server.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Linked Service SQL Server. Changing this forces a new resource</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_sql_server.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_linked_service_sql_server.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.LinkedServiceSqlServer.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.LinkedServiceSqlServer.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.Pipeline">
<em class="property">class </em><code class="descclassname">pulumi_azure.datafactory.</code><code class="descname">Pipeline</code><span class="sig-paren">(</span><em>resource_name</em>, <em>opts=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>variables=None</em>, <em>__props__=None</em>, <em>__name__=None</em>, <em>__opts__=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline" title="Permalink to this definition">¶</a></dt>
<dd><p>Manage a Pipeline inside a Azure Data Factory.</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</li>
<li><strong>annotations</strong> (<em>pulumi.Input</em><em>[</em><em>list</em><em>]</em>) – List of tags that can be used for describing the Data Factory Pipeline.</li>
<li><strong>data_factory_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The Data Factory name in which to associate the Pipeline with. Changing this forces a new resource.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The description for the Data Factory Pipeline.</li>
<li><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>Specifies the name of the Data Factory Pipeline. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</li>
<li><strong>parameters</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of parameters to associate with the Data Factory Pipeline.</li>
<li><strong>resource_group_name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The name of the resource group in which to create the Data Factory Pipeline. Changing this forces a new resource</li>
<li><strong>variables</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A map of variables to associate with the Data Factory Pipeline.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_pipeline.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_pipeline.html.markdown</a>.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_azure.datafactory.Pipeline.annotations">
<code class="descname">annotations</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.annotations" title="Permalink to this definition">¶</a></dt>
<dd><p>List of tags that can be used for describing the Data Factory Pipeline.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Pipeline.data_factory_name">
<code class="descname">data_factory_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.data_factory_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The Data Factory name in which to associate the Pipeline with. Changing this forces a new resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Pipeline.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.description" title="Permalink to this definition">¶</a></dt>
<dd><p>The description for the Data Factory Pipeline.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Pipeline.name">
<code class="descname">name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.name" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies the name of the Data Factory Pipeline. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Pipeline.parameters">
<code class="descname">parameters</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.parameters" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of parameters to associate with the Data Factory Pipeline.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Pipeline.resource_group_name">
<code class="descname">resource_group_name</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.resource_group_name" title="Permalink to this definition">¶</a></dt>
<dd><p>The name of the resource group in which to create the Data Factory Pipeline. Changing this forces a new resource</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_azure.datafactory.Pipeline.variables">
<code class="descname">variables</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.variables" title="Permalink to this definition">¶</a></dt>
<dd><p>A map of variables to associate with the Data Factory Pipeline.</p>
</dd></dl>

<dl class="staticmethod">
<dt id="pulumi_azure.datafactory.Pipeline.get">
<em class="property">static </em><code class="descname">get</code><span class="sig-paren">(</span><em>resource_name</em>, <em>id</em>, <em>opts=None</em>, <em>annotations=None</em>, <em>data_factory_name=None</em>, <em>description=None</em>, <em>name=None</em>, <em>parameters=None</em>, <em>resource_group_name=None</em>, <em>variables=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Pipeline resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.
:param str resource_name: The unique name of the resulting resource.
:param str id: The unique provider ID of the resource to lookup.
:param pulumi.ResourceOptions opts: Options for the resource.
:param pulumi.Input[list] annotations: List of tags that can be used for describing the Data Factory Pipeline.
:param pulumi.Input[str] data_factory_name: The Data Factory name in which to associate the Pipeline with. Changing this forces a new resource.
:param pulumi.Input[str] description: The description for the Data Factory Pipeline.
:param pulumi.Input[str] name: Specifies the name of the Data Factory Pipeline. Changing this forces a new resource to be created. Must be globally unique. See the <a class="reference external" href="https://docs.microsoft.com/en-us/azure/data-factory/naming-rules">Microsoft documentation</a> for all restrictions.
:param pulumi.Input[dict] parameters: A map of parameters to associate with the Data Factory Pipeline.
:param pulumi.Input[str] resource_group_name: The name of the resource group in which to create the Data Factory Pipeline. Changing this forces a new resource
:param pulumi.Input[dict] variables: A map of variables to associate with the Data Factory Pipeline.</p>
<blockquote>
<div>This content is derived from <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_pipeline.html.markdown">https://github.com/terraform-providers/terraform-provider-azurerm/blob/master/website/docs/r/data_factory_pipeline.html.markdown</a>.</div></blockquote>
</dd></dl>

<dl class="method">
<dt id="pulumi_azure.datafactory.Pipeline.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.translate_output_property" title="Permalink to this definition">¶</a></dt>
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
<dt id="pulumi_azure.datafactory.Pipeline.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_azure.datafactory.Pipeline.translate_input_property" title="Permalink to this definition">¶</a></dt>
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
