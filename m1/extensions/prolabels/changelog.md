---
layout: default
title: Changelog
description: Product Labels Changelog
keywords: prolabels changelog, product labls changelog
category: Prolabels
---

# Changelog

### Version 2.7.16

> Sep 30, 2019

 -  Remove limit from label styles and label text length.
 -  Do not show system labels for all stores while it's enabled for one only.

### Version 2.7.15

> Feb 26, 2019

 -  Fix Integrity constraint violation error for manual labels when Customer Groups filter is enabled.

### Version 2.7.14

  -  Use unified image uploader from TM Core in admin interfaces.

### Version 2.7.13

 -  Added new position for label - ‘hidden’. With this position you can hide label on product page or category page.

### Version 2.7.12

 -  Escape quotes in lable's title.
 -  Prevent label wrapper from stretching out of parent container.
 -  Significant code cleanup and code improvement.

You can safely remove follow directories and files to keep your Magento
instance "clean and tidy":

```
app/code/local/TM/ProLabels/Adminhtml
app/code/local/TM/ProLabels/Block/Adminhtml/System/Edit/Tab
app/code/local/TM/ProLabels/Block/Adminhtml/System/Grid
app/code/local/TM/ProLabels/Block/Adminhtml/System/Helper
app/code/local/TM/ProLabels/Block/Adminhtml/System/Widget
app/code/local/TM/ProLabels/Model/Entity/Attribute/Backend
app/code/local/TM/ProLabels/Model/System/Config/Source

app/code/local/TM/ProLabels/Block/Adminhtml/System/Edit/Form.php

```

### Version 2.7.11

 -  Fixed missing labels when enabled option 'Move to content on mobile'.
 -  Do not render empty container for content labels if there are no labels.
 -  PHP code cleanup to pass MEQP validation

### Version 2.7.8

 -  Fix notice "Undefined variable" when stock labels render.
 -  Improved backend interfaces.
 -  Include Mobile_detect lib only if it is nessecery.
 -  Image validator added for Magento 1.9.3.3.

### Version 2.7.6

 -  slightly improved content labels template
 -  remove deprecated IE6 styles

### Version 2.7.4

 -  JS file loads and executes with *defer* attribute, so it does not block
    page rendering
 -  no more inline javascript in templates
 -  significantly reduced html content generated by extension
 -  minor style improvements for content labels
 -  refactored and unified template for content labels
 -  fixed notices in Magento log about tooltips for content labels
 -  fixed notices in Magento log for bundle and grouped products with
    "on sale" labels

You can safely remove follow directories to keep your Magento instance "clean and tidy":

```
app/design/frontend/base/default/template/tm/prolabels/category
app/design/frontend/base/default/template/tm/prolabels/product
app/design/frontend/base/default/template/tm/prolabels/rules
```

### Version 2.7.3

 -  Fatal error: Cannot break/continue 1 level
 -  Validate store, when enable labels priority

### Version 2.7.2

 -  Added ability to render prolabels programmatically from third-party
    modules with *prolabels_get_label_html_after* event. (See
    [tm/dailydeals](https://github.com/tmhub/dailydeals) module)
 -  Compatibility with modules that use Mobile_Detect class

### Version 2.7.1

 -  add custom url option to content labels
 -  Magento 1.9.2.0 compatibility added

### Version 2.7.0

 -  add alt for label links
 -  add support labels custom url( only product image labels )
 -  add to module configuration enable/disable indexin label with cron
 -  create prolabels shell script
    ``` php
    php -f prolabels.php -- reindex
    ```
 -  filter labels by customer groups
 -  fix calculate product special price for bundle product
 -  fix show stock item variable for manual labels


