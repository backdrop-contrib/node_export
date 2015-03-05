Node export
===========

This module allows users to export nodes and then import them into another
Backdrop installation, or on the same site.

Requirement
-----------

This module needs the UUID module to be installed and enabled in order to
function.

Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules

- Visit admin/build/modules to enable the Node export module in the Node export
   package.

- Enable permissions at admin/user/permissions.

      Security Warning: Users with the permission "use PHP to import nodes"
      will be able to change nodes as they see fit before an import, as well as
      being able to execute PHP scripts on the server.  It is advisable not to
      give this permission to a typical node author, only the administrator or
      developer should use this feature.  You may even like to turn this module
      off when it is no longer required.
      This module does not check access to the filter formats used by the node's
      fields, please keep this in mind when assigning permissions to user roles.
- Configure module at admin/settings/node_export.


USAGE
-----
To export nodes, use the 'Node export' tab on a node page. Or, use the Find
content page (admin/content) to filter the nodes you wish to export and then
choose 'Node export' under the 'Update options'.


To import nodes that were exported with Node export,  use the form at 'Node
export: import' under 'Add content' (node/add/node_export).

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.

Current Maintainers
-------------------

- Luke McCormick (https://github.com/cellear/)

Credits
-------

This module is based on the Drupal module Node Export

Project page: http://drupal.org/project/node_export.

Drupal Maintainer: Daniel Braksator (http://drupal.org/user/134005)

Note: this module was originally built upon code from the node_clone module
maintained by Peter Wolanin (http://drupal.org/user/49851) at
http://drupal.org/project/node_clone which was derived from code posted by
Steve Ringwood (http://drupal.org/user/12856) at
http://drupal.org/node/73381#comment-137714
Features integration, relations, and UUID initially developed by Tushar Mahajan
(http://drupal.org/user/398572).
Significant improvements, file handling, and extra functionality pioneered by
James Andres (http://drupal.org/user/33827).
