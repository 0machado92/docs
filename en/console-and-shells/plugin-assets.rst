Plugin Assets Shell
###################

CakePHP by default serves plugins assets using the ``AssetFilter`` dispatcher
filter. While this is a good convenience, it is recommended to symlink / copy
the plugin assets under app's webroot so that they can be directly served by the
web server without invoking PHP. You can do this by running::

    bin/cake plugin_assets symlink

Running the above command will symlink all plugins assets under app's webroot.
On Windows, which doesn't support symlinks, the assets will be copied in
respective folders instead of being symlinked.

.. meta::
    :title lang=en: Plugin Assets Shell
    :keywords lang=en: plugin,assets
