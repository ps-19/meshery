---
layout: default
title: stop
permalink: reference/mesheryctl/system/stop
type: reference
display-title: "false"
language: en
lang: en
categories: en
list: exclude
# image: /assets/img/platforms/brew.png
---

<!-- Copy this template to create individual doc pages for each mesheryctl commands -->

<!-- Name of the command -->
# mesheryctl system stop

## Description

{% for subcommand_hash in site.data.mesheryctlcommands.lifecycle.system.stop.command %}{% assign subcommand = subcommand_hash[1] %}
{{ subcommand.description }}
{% endfor %}

<!-- Basic usage of the command -->
<pre class="codeblock-pre">
  <div class="codeblock">
    mesheryctl system stop [flags]
  </div>
</pre>

## Examples

<pre class="codeblock-pre">
  <div class="codeblock">
  {% for subcommand_hash in site.data.mesheryctlcommands.lifecycle.system.stop.command %}{% assign subcommand = subcommand_hash[1] %}
  # {{ subcommand.description }}
  {{ subcommand.usage }}
  {% endfor %}
  {% for flag_hash in site.data.mesheryctlcommands.lifecycle.system.stop.flag %}{% assign flag = flag_hash[1] %}
  # {{ flag.description }}
  {{ flag.usage }}
  {% endfor %}
  </div>
</pre>
<br/>


<!-- Options/Flags available in this command -->
## Options

<pre class="codeblock-pre">
  <div class="codeblock">
    {% for flag_hash in site.data.mesheryctlcommands.lifecycle.system.stop.flag %}{% assign flag = flag_hash[1] %}
    {{ flag.flag }} # {{ flag.description }}
    {% endfor %}
  </div>
</pre>
<br/>