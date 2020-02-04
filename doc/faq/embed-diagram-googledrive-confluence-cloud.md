---
title: How to embed a diagram from Google Drive into Confluence Cloud
layout: page
faq: true
categories: [Confluence Cloud]
---

Use the _Embed draw.io diagram_ macro to connect to Google Drive and embed a .drawio diagram file hosted there.

1. Edit the Confluence page on which you want to embed your diagram, then type ``/draw`` to insert a macro. Select _Embed draw.io diagram_.
2. Click the _Google Drive_ tab. If you haven't allowed draw.io to access your files on Google Drive, click the blue _Authorize_ button, and follow the prompts to allow access.
3. When you return to the file picker, click _Choose_.
<br /><img src="/assets/img/blog/choose-diagram-google-drive-confluence-cloud.png" width="400" alt="Click Choose to look for the .drawio diagram file in your Google Drive">
4. Find and click on .drawio diagram file you want to embed, then click on the blue _Select_ button.
<br /><img src="/assets/img/blog/select-diagram-google-drive-confluence-cloud.png" width="400" alt="Select the draw.io diagram file in your Google Drive">
5. Check the preview to make sure you have the right diagram, then click _Select_.
<br /><img src="/assets/img/blog/select-preview-google-drive-confluence-cloud.png" width="400" alt="Check the preview of your .drawio diagram file on Google Drive">
6. Finally, click _Insert_ to embed your diagram file from Google Drive into your Confluence Cloud page.
<br /><img src="/assets/img/blog/insert-google-drive-confluence-cloud.png" width="400" alt="Click Insert to embed the diagram file from your Google Drive into your Confluence Cloud page">

## What happens to embedded diagrams if draw.io is uninstalled?

The embedded diagrams and files in Confluence or Jira will no longer be able to be displayed. In Confluence, this will be displayed as if the macro is broken (no macros are deleted though). Of course, no data on Google Drive is deleted!

When you reinstall the Diagram Viewer app, as long as the connection with Google Drive is still authorised, your diagrams and files will be displayed again, no further steps necessary.

**Tip:** You can also [embed diagrams from OneDrive](/doc/faq/embed-diagram-googledrive-confluence-cloud.html) and [other Confluence pages](/doc/faq/embed-copy-move-diagrams-Confluence-Cloud.md).

<img src="/assets/img/blog/embed-diagrams-confluence-cloud.png" width="600" alt="Embedded diagrams in draw.io for Confluence Cloud">
