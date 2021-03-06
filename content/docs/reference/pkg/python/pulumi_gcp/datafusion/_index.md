---
title: Module datafusion
title_tag: Module datafusion | Package pulumi_gcp | Python SDK
linktitle: datafusion
notitle: true
block_external_search_index: true
---

{{< resource-docs-alert "gcp" >}}

<div class="section" id="datafusion">
<h1>datafusion<a class="headerlink" href="#datafusion" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div><p>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-gcp/issues">pulumi/pulumi-gcp repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-google/issues">terraform-providers/terraform-provider-google repo</a>.</p>
</div></blockquote>
<span class="target" id="module-pulumi_gcp.datafusion"></span><dl class="py class">
<dt id="pulumi_gcp.datafusion.Instance">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_gcp.datafusion.</code><code class="sig-name descname">Instance</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span></em>, <em class="sig-param"><span class="n">opts</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">description</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">enable_stackdriver_logging</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">enable_stackdriver_monitoring</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">labels</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">network_config</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">options</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">private_instance</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">project</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">region</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">type</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.datafusion.Instance" title="Permalink to this definition">¶</a></dt>
<dd><p>Represents a Data Fusion instance.</p>
<p>To get more information about Instance, see:</p>
<ul class="simple">
<li><p><a class="reference external" href="https://cloud.google.com/data-fusion/docs/reference/rest/v1beta1/projects.locations.instances">API documentation</a></p></li>
<li><p>How-to Guides</p>
<ul>
<li><p><a class="reference external" href="https://cloud.google.com/data-fusion/docs/">Official Documentation</a></p></li>
</ul>
</li>
</ul>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_gcp</span> <span class="k">as</span> <span class="nn">gcp</span>

<span class="n">basic_instance</span> <span class="o">=</span> <span class="n">gcp</span><span class="o">.</span><span class="n">datafusion</span><span class="o">.</span><span class="n">Instance</span><span class="p">(</span><span class="s2">&quot;basicInstance&quot;</span><span class="p">,</span>
    <span class="n">region</span><span class="o">=</span><span class="s2">&quot;us-central1&quot;</span><span class="p">,</span>
    <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;BASIC&quot;</span><span class="p">)</span>
</pre></div>
</div>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_gcp</span> <span class="k">as</span> <span class="nn">gcp</span>

<span class="n">extended_instance</span> <span class="o">=</span> <span class="n">gcp</span><span class="o">.</span><span class="n">datafusion</span><span class="o">.</span><span class="n">Instance</span><span class="p">(</span><span class="s2">&quot;extendedInstance&quot;</span><span class="p">,</span>
    <span class="n">description</span><span class="o">=</span><span class="s2">&quot;My Data Fusion instance&quot;</span><span class="p">,</span>
    <span class="n">enable_stackdriver_logging</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
    <span class="n">enable_stackdriver_monitoring</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
    <span class="n">labels</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;example_key&quot;</span><span class="p">:</span> <span class="s2">&quot;example_value&quot;</span><span class="p">,</span>
    <span class="p">},</span>
    <span class="n">network_config</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;ipAllocation&quot;</span><span class="p">:</span> <span class="s2">&quot;10.89.48.0/22&quot;</span><span class="p">,</span>
        <span class="s2">&quot;network&quot;</span><span class="p">:</span> <span class="s2">&quot;default&quot;</span><span class="p">,</span>
    <span class="p">},</span>
    <span class="n">private_instance</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
    <span class="n">region</span><span class="o">=</span><span class="s2">&quot;us-central1&quot;</span><span class="p">,</span>
    <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;BASIC&quot;</span><span class="p">)</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An optional description of the instance.</p></li>
<li><p><strong>enable_stackdriver_logging</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Option to enable Stackdriver Logging.</p></li>
<li><p><strong>enable_stackdriver_monitoring</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Option to enable Stackdriver Monitoring.</p></li>
<li><p><strong>labels</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – The resource labels for instance to use to annotate any related underlying resources,
such as Compute Engine VMs.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the instance or a fully qualified identifier for the instance.</p></li>
<li><p><strong>network_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Network configuration options. These are required when a private Data Fusion instance is to be created.  Structure is documented below.</p></li>
<li><p><strong>options</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Map of additional options used to configure the behavior of Data Fusion instance.</p></li>
<li><p><strong>private_instance</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Specifies whether the Data Fusion instance should be private. If set to
true, all Data Fusion nodes will have private IP addresses and will not be
able to access the public internet.</p></li>
<li><p><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</p></li>
<li><p><strong>region</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The region of the Data Fusion instance.</p></li>
<li><p><strong>type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Represents the type of Data Fusion instance. Each type is configured with
the default settings for processing and memory.</p></li>
</ul>
</dd>
</dl>
<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">-</span> <span class="n">BASIC</span><span class="p">:</span> <span class="n">Basic</span> <span class="n">Data</span> <span class="n">Fusion</span> <span class="n">instance</span><span class="o">.</span> <span class="n">In</span> <span class="n">Basic</span> <span class="nb">type</span><span class="p">,</span> <span class="n">the</span> <span class="n">user</span> <span class="n">will</span> <span class="n">be</span> <span class="n">able</span> <span class="n">to</span> <span class="n">create</span> <span class="n">data</span> <span class="n">pipelines</span>
<span class="n">using</span> <span class="n">point</span> <span class="ow">and</span> <span class="n">click</span> <span class="n">UI</span><span class="o">.</span> <span class="n">However</span><span class="p">,</span> <span class="n">there</span> <span class="n">are</span> <span class="n">certain</span> <span class="n">limitations</span><span class="p">,</span> <span class="n">such</span> <span class="k">as</span> <span class="n">fewer</span> <span class="n">number</span>
<span class="n">of</span> <span class="n">concurrent</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">no</span> <span class="n">support</span> <span class="k">for</span> <span class="n">streaming</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">etc</span><span class="o">.</span>
<span class="o">-</span> <span class="n">ENTERPRISE</span><span class="p">:</span> <span class="n">Enterprise</span> <span class="n">Data</span> <span class="n">Fusion</span> <span class="n">instance</span><span class="o">.</span> <span class="n">In</span> <span class="n">Enterprise</span> <span class="nb">type</span><span class="p">,</span> <span class="n">the</span> <span class="n">user</span> <span class="n">will</span> <span class="n">have</span> <span class="n">more</span> <span class="n">features</span>
<span class="n">available</span><span class="p">,</span> <span class="n">such</span> <span class="k">as</span> <span class="n">support</span> <span class="k">for</span> <span class="n">streaming</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">higher</span> <span class="n">number</span> <span class="n">of</span> <span class="n">concurrent</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">etc</span><span class="o">.</span>
</pre></div>
</div>
<p>The <strong>network_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">ipAllocation</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The IP range in CIDR notation to use for the managed Data Fusion instance
nodes. This range must not overlap with any other ranges used in the Data Fusion instance network.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">network</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Name of the network in the project with which the tenant project
will be peered for executing pipelines. In case of shared VPC where the network resides in another host
project the network should specified in the form of projects/{host-project-id}/global/networks/{network}</p></li>
</ul>
<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.create_time">
<code class="sig-name descname">create_time</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.create_time" title="Permalink to this definition">¶</a></dt>
<dd><p>The time the instance was created in RFC3339 UTC “Zulu” format, accurate to nanoseconds.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.description">
<code class="sig-name descname">description</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.description" title="Permalink to this definition">¶</a></dt>
<dd><p>An optional description of the instance.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.enable_stackdriver_logging">
<code class="sig-name descname">enable_stackdriver_logging</code><em class="property">: pulumi.Output[bool]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.enable_stackdriver_logging" title="Permalink to this definition">¶</a></dt>
<dd><p>Option to enable Stackdriver Logging.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.enable_stackdriver_monitoring">
<code class="sig-name descname">enable_stackdriver_monitoring</code><em class="property">: pulumi.Output[bool]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.enable_stackdriver_monitoring" title="Permalink to this definition">¶</a></dt>
<dd><p>Option to enable Stackdriver Monitoring.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.labels">
<code class="sig-name descname">labels</code><em class="property">: pulumi.Output[dict]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.labels" title="Permalink to this definition">¶</a></dt>
<dd><p>The resource labels for instance to use to annotate any related underlying resources,
such as Compute Engine VMs.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.name">
<code class="sig-name descname">name</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the instance or a fully qualified identifier for the instance.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.network_config">
<code class="sig-name descname">network_config</code><em class="property">: pulumi.Output[dict]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.network_config" title="Permalink to this definition">¶</a></dt>
<dd><p>Network configuration options. These are required when a private Data Fusion instance is to be created.  Structure is documented below.</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">ipAllocation</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - The IP range in CIDR notation to use for the managed Data Fusion instance
nodes. This range must not overlap with any other ranges used in the Data Fusion instance network.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">network</span></code> (<code class="docutils literal notranslate"><span class="pre">str</span></code>) - Name of the network in the project with which the tenant project
will be peered for executing pipelines. In case of shared VPC where the network resides in another host
project the network should specified in the form of projects/{host-project-id}/global/networks/{network}</p></li>
</ul>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.options">
<code class="sig-name descname">options</code><em class="property">: pulumi.Output[dict]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.options" title="Permalink to this definition">¶</a></dt>
<dd><p>Map of additional options used to configure the behavior of Data Fusion instance.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.private_instance">
<code class="sig-name descname">private_instance</code><em class="property">: pulumi.Output[bool]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.private_instance" title="Permalink to this definition">¶</a></dt>
<dd><p>Specifies whether the Data Fusion instance should be private. If set to
true, all Data Fusion nodes will have private IP addresses and will not be
able to access the public internet.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.project">
<code class="sig-name descname">project</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.region">
<code class="sig-name descname">region</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.region" title="Permalink to this definition">¶</a></dt>
<dd><p>The region of the Data Fusion instance.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.service_account">
<code class="sig-name descname">service_account</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.service_account" title="Permalink to this definition">¶</a></dt>
<dd><p>Service account which will be used to access resources in the customer project.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.service_endpoint">
<code class="sig-name descname">service_endpoint</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.service_endpoint" title="Permalink to this definition">¶</a></dt>
<dd><p>Endpoint on which the Data Fusion UI and REST APIs are accessible.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.state">
<code class="sig-name descname">state</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.state" title="Permalink to this definition">¶</a></dt>
<dd><p>The current state of this Data Fusion instance. - CREATING: Instance is being created - RUNNING: Instance is running and
ready for requests - FAILED: Instance creation failed - DELETING: Instance is being deleted - UPGRADING: Instance is
being upgraded - RESTARTING: Instance is being restarted</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.state_message">
<code class="sig-name descname">state_message</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.state_message" title="Permalink to this definition">¶</a></dt>
<dd><p>Additional information about the current state of this Data Fusion instance if available.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.type">
<code class="sig-name descname">type</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.type" title="Permalink to this definition">¶</a></dt>
<dd><p>Represents the type of Data Fusion instance. Each type is configured with
the default settings for processing and memory.</p>
<ul class="simple">
<li><p>BASIC: Basic Data Fusion instance. In Basic type, the user will be able to create data pipelines
using point and click UI. However, there are certain limitations, such as fewer number
of concurrent pipelines, no support for streaming pipelines, etc.</p></li>
<li><p>ENTERPRISE: Enterprise Data Fusion instance. In Enterprise type, the user will have more features
available, such as support for streaming pipelines, higher number of concurrent pipelines, etc.</p></li>
</ul>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.update_time">
<code class="sig-name descname">update_time</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.update_time" title="Permalink to this definition">¶</a></dt>
<dd><p>The time the instance was last updated in RFC3339 UTC “Zulu” format, accurate to nanoseconds.</p>
</dd></dl>

<dl class="py attribute">
<dt id="pulumi_gcp.datafusion.Instance.version">
<code class="sig-name descname">version</code><em class="property">: pulumi.Output[str]</em><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.version" title="Permalink to this definition">¶</a></dt>
<dd><p>Current version of the Data Fusion.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_gcp.datafusion.Instance.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span></em>, <em class="sig-param"><span class="n">id</span></em>, <em class="sig-param"><span class="n">opts</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">create_time</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">description</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">enable_stackdriver_logging</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">enable_stackdriver_monitoring</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">labels</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">network_config</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">options</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">private_instance</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">project</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">region</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_account</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_endpoint</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">state</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">state_message</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">type</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">update_time</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">version</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Instance resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>str</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>create_time</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The time the instance was created in RFC3339 UTC “Zulu” format, accurate to nanoseconds.</p></li>
<li><p><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An optional description of the instance.</p></li>
<li><p><strong>enable_stackdriver_logging</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Option to enable Stackdriver Logging.</p></li>
<li><p><strong>enable_stackdriver_monitoring</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Option to enable Stackdriver Monitoring.</p></li>
<li><p><strong>labels</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – The resource labels for instance to use to annotate any related underlying resources,
such as Compute Engine VMs.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the instance or a fully qualified identifier for the instance.</p></li>
<li><p><strong>network_config</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Network configuration options. These are required when a private Data Fusion instance is to be created.  Structure is documented below.</p></li>
<li><p><strong>options</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – Map of additional options used to configure the behavior of Data Fusion instance.</p></li>
<li><p><strong>private_instance</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Specifies whether the Data Fusion instance should be private. If set to
true, all Data Fusion nodes will have private IP addresses and will not be
able to access the public internet.</p></li>
<li><p><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.</p></li>
<li><p><strong>region</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The region of the Data Fusion instance.</p></li>
<li><p><strong>service_account</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Service account which will be used to access resources in the customer project.</p></li>
<li><p><strong>service_endpoint</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Endpoint on which the Data Fusion UI and REST APIs are accessible.</p></li>
<li><p><strong>state</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The current state of this Data Fusion instance. - CREATING: Instance is being created - RUNNING: Instance is running and
ready for requests - FAILED: Instance creation failed - DELETING: Instance is being deleted - UPGRADING: Instance is
being upgraded - RESTARTING: Instance is being restarted</p></li>
<li><p><strong>state_message</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Additional information about the current state of this Data Fusion instance if available.</p></li>
<li><p><strong>type</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Represents the type of Data Fusion instance. Each type is configured with
the default settings for processing and memory.</p></li>
</ul>
</dd>
</dl>
<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">-</span> <span class="n">BASIC</span><span class="p">:</span> <span class="n">Basic</span> <span class="n">Data</span> <span class="n">Fusion</span> <span class="n">instance</span><span class="o">.</span> <span class="n">In</span> <span class="n">Basic</span> <span class="nb">type</span><span class="p">,</span> <span class="n">the</span> <span class="n">user</span> <span class="n">will</span> <span class="n">be</span> <span class="n">able</span> <span class="n">to</span> <span class="n">create</span> <span class="n">data</span> <span class="n">pipelines</span>
<span class="n">using</span> <span class="n">point</span> <span class="ow">and</span> <span class="n">click</span> <span class="n">UI</span><span class="o">.</span> <span class="n">However</span><span class="p">,</span> <span class="n">there</span> <span class="n">are</span> <span class="n">certain</span> <span class="n">limitations</span><span class="p">,</span> <span class="n">such</span> <span class="k">as</span> <span class="n">fewer</span> <span class="n">number</span>
<span class="n">of</span> <span class="n">concurrent</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">no</span> <span class="n">support</span> <span class="k">for</span> <span class="n">streaming</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">etc</span><span class="o">.</span>
<span class="o">-</span> <span class="n">ENTERPRISE</span><span class="p">:</span> <span class="n">Enterprise</span> <span class="n">Data</span> <span class="n">Fusion</span> <span class="n">instance</span><span class="o">.</span> <span class="n">In</span> <span class="n">Enterprise</span> <span class="nb">type</span><span class="p">,</span> <span class="n">the</span> <span class="n">user</span> <span class="n">will</span> <span class="n">have</span> <span class="n">more</span> <span class="n">features</span>
<span class="n">available</span><span class="p">,</span> <span class="n">such</span> <span class="k">as</span> <span class="n">support</span> <span class="k">for</span> <span class="n">streaming</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">higher</span> <span class="n">number</span> <span class="n">of</span> <span class="n">concurrent</span> <span class="n">pipelines</span><span class="p">,</span> <span class="n">etc</span><span class="o">.</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>update_time</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The time the instance was last updated in RFC3339 UTC “Zulu” format, accurate to nanoseconds.</p></li>
<li><p><strong>version</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Current version of the Data Fusion.</p></li>
</ul>
</dd>
</dl>
<p>The <strong>network_config</strong> object supports the following:</p>
<ul class="simple">
<li><p><code class="docutils literal notranslate"><span class="pre">ipAllocation</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - The IP range in CIDR notation to use for the managed Data Fusion instance
nodes. This range must not overlap with any other ranges used in the Data Fusion instance network.</p></li>
<li><p><code class="docutils literal notranslate"><span class="pre">network</span></code> (<code class="docutils literal notranslate"><span class="pre">pulumi.Input[str]</span></code>) - Name of the network in the project with which the tenant project
will be peered for executing pipelines. In case of shared VPC where the network resides in another host
project the network should specified in the form of projects/{host-project-id}/global/networks/{network}</p></li>
</ul>
</dd></dl>

<dl class="py method">
<dt id="pulumi_gcp.datafusion.Instance.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_gcp.datafusion.Instance.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.datafusion.Instance.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

</div>
