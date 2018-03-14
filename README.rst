Vimeo Plugin for CKEditor 4
===========================

This plugin allow you to insert Vimeo videos using embed code or just the video URL.

Installation
************

With NPM
--------

1. npm install ckeditor-vimeo-plugin
2. Add the plugin to CKEditor (config.js):

    ::

        CKEDITOR.plugins.addExternal('vimeo', '../node_modules/ckeditor-vimeo-plugin/vimeo/');

        config.extraPlugins = 'vimeo';

    You may need to adjust the plugin path. The example is assuming that you have the following directory structure: ::

        project
        └───ckeditor
        │   └───config.js
        └───node_modules
            └───ckeditor-vimeo-plugin

Manual
------

Follow these steps:

1. Download the latest version of the plugin from Github.
2. Extract the downloaded file into the CKEditor's **plugins** folder.
3. Enable the plugin by changing or adding the extraPlugins line in your configuration (config.js): ::

    config.extraPlugins = 'vimeo';


Configuration
*************

The default options can be overriden on config.js.

Video width
    ::

        config.vimeo_width = '640';

Video height
    ::

        config.vimeo_height = '480';

Make responsive (ignore width and height, fit to width):
    ::

        config.vimeo_responsive = true;

Start video automatically
    ::

        config.vimeo_autoplay = false;

Disable the change of settings
    The elements on the list will be disabled (but still visible).

    ::

        config.vimeo_disabled_fields = ['txtEmbed', 'chkAutoplay'];

    See the available element list below.


List of UI elements
-------------------

* txtEmbed
* txtUrl
* txtWidth
* txtHeight
* chkResponsive
* chkAutoplay


How to use
**********

If everything is ok, a Vimeo icon should appear on the CKEditor toolbar. Click it,
paste your embed code or video URL and the video will be inserted.

Credits
*******

This project has been started and modified from original project `ckeditor-youtube-plugin <https://github.com/fonini/ckeditor-youtube-plugin>`_ version 2.1.10 from `Jonnas Fonini <https://github.com/fonini/ckeditor-youtube-plugin>`_.

And it is licensed under the `WTFPL <http://www.wtfpl.net>`_ to respect original project license.
