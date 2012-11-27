octopress-facebook-likebox
==========================

A simple Octopress aside and plugin to display a Facebook likebox for a Facebook page

Based on the HTML5 implementation of the [Facebook Likebox](http://developers.Facebook.com/docs/reference/plugins/like-box/)

###Install Instructions
1. Copy `likebox.rb` to your `plugins` directory
2. Copy `likebox.html` to your `source/_includes/asides` directory
3. Add the following to the top of your `source/_layouts/default.html`
  {% if site.Facebook_pagename %}
    {% likebox %}
  {% endif %}
4. Add configuration info to `_config.yml`

###Configuring Facebook likebox
There are a number of optional parameters relating to the display of the likebox. They are fully documented at the Facebook developer's website above, but here is a brief overview

**facebook_pagename**
This is required. If your Facebook page is www.Facebook.com/mycoolpage, then the `Facebook_pagename` would be `mycoolpage`

**facebook_showfaces**
Will display the faces of people who have liked the page on Facebook. 

**facebook_showstream**
Will stream the latest posts from your page.

**facebook_bordercolor**
Change the color of the border of the likebox (in hex). This parameter is not required.

**facebook_darktheme**
Set to true to change to a darker theme for the likebox.

**facebook_height**
Manually set the height for the likebox.

**facebook_width**
Manually set the width for the likebox. Facebook will default the width to 292px. If you're using the default Octopress theme, set the width to 260px for it to fit in the aside area.

###Example config:

 \# Facebook likebox (for pages)
  facebook_pagename: MyCoolPage
  facebook_showfaces: true
  facebook_showstream: true
  facebook_width: 260

###Send feedback

This is my first Octopress plugin! Am I doing it wrong?
