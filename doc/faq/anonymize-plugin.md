---
title: How to use the anonymize plugin to scramble all text in your diagram
layout: page
faq: true
categories: [Plugins, Confluence Cloud, Confluence Server]
---

If you need to remove confidential, sensitive or identifying information before sharing your diagrams, use the anonymize plugin. This plugin will scramble all of the text and metadata in your diagram.

[More information about diagrams.net plugins](/doc/faq/plugins.html)

## Load the anonymize plugin
* To create a new diagram with the plugin already loaded, go to [https://app.diagrams.net/?splash=0&p=anon](https://app.diagrams.net/?splash=0&p=anon)

## Anonymise your diagram content

Once you have loaded the anonymize plugin, the _Anonymize Current Page_ menu entry will let you scramble the text and metadata in your diagram. This includes all labels and shape metadata on that page, and the page's name.

* On each page in your diagram, click _Extras > Anonymize Current Page_.

**Before anonymising your diagram**

<img src="/assets/img/blog/extras-anonymize-current-page.png" width="600" alt="Click Extras > Anonymize Current Page to scramble all of the text on that page">

**After anonymising your diagram**

<img src="/assets/img/blog/anonymized-diagram.png" width="600" alt="All text has been scrambed, including the page name and shape metadata">

## Permanently load the plugin

If you need to anonymise diagrams regularly, add the anonymize plugin to the plugins list to load it each time you create or edit a diagram.

1. From the menu, select _Extras > Plugins_.
<br /><img src="/assets/img/blog/extras-plugins.png" width="400" alt="Open the plugins list">
2. Click _Add_.
<br /><img src="/assets/img/blog/add-plugin.png" width="200" alt="Add a new plugin">
2. Paste ``/plugins/anonymize.js`` into the URL field, then click _Add_
<br /><img src="/assets/img/blog/add-anonymize-plugin.png" width="200" alt="Add the anonymize plugin">
3. Click _Apply_.
<br /><img src="/assets/img/blog/apply-add-anonymize-plugin.png" width="200" alt="Add the anonymize plugin">

### Load the anonymize plugin on Confluence Server

Administrators can add the anonymize plugin to draw.io in Confluence Server via the draw.io configuration.

1. [Download the anonymize plugin from GitHub](https://raw.githubusercontent.com/jgraph/drawio/618eff1544e7c763d12219cba21d8256044d6a1d/war/plugins/anonymize.js) and attach it to a page in your instance.
2. As an administrator, go to the _draw.io Configuration_ section, in the left-hand menu of your Confluence Settings. Click on the Configuration tab.
2. Add the plugins option to the JSON code in the UI configuration. Use the relative URL to the attachment you saved in step 1. For example: ``"plugins": [ "/download/attachments/55279729/anonymize.js" ]``
<br /><img src="/assets/img/blog/add-anonymize-plugin-confluence-server.png" width="400" alt="Add the anonymize plugin to draw.io in Confluence Server">
3. Click _Save Changes_.

### Load the anonymize plugin on Confluence Cloud

To ensure security, you are limited to the official plugins in draw.io for Confluence Cloud. Instead of attaching the JavaScript file to a page, an administrator can add the plugin ID for the anonymize plugin, ``anon``, to the JSON configuration code.

1. Go to the _draw.io Configuration_ tab in the _draw.io Configuration_ section of your Confluence Cloud settings.
2. As an administrator, add ``{ "plugins": ["anon"] }`` to the JSON code.
<br /><img src="/assets/img/blog/add-anon-plugin-confluence-cloud.png" width="400" alt="Add the anonymize plugin to draw.io in Confluence Cloud">
3. Click _Save_.

[Learn more about loading plugins in Confluence Cloud](/doc/faq/custom-plugins-confluence-cloud.html)
