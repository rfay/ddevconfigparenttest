This repo is just for testing and experimentation with
https://github.com/ddev/ddev/issues/6937

It's a basic Drupal 11 project.

* It has a post-start hook to install the issue-reported problem (`composer require --dev drupal/svg_image_field:dev-2.3.x`). (It's hard to check that into git because it's git and not doing as a submodule)
* You probably don't need a fully functional site, but there are database and files in the .tarballs directory that can be used for `ddev import-db` and `ddev import-files`

We should be able to demonstrate all the problems by experimenting with this project with or without its main config.yaml, and with or without the .ddev directory in web/modules/contrib/svg_image_field
