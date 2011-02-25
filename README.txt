
Node export README

CONTENTS OF THIS FILE
----------------------

  * Introduction
  * Installation
  * Configuration
  * Usage


INTRODUCTION
------------
This module allows users to export nodes and then import it into another
Drupal installation, or on the same site.

This module allows user to export/import nodes if they have the 'export nodes'
or 'export own nodes' permission, have node access to view the node and create
the node type, and the node type is not omitted in node export's settings. The
module does not check access to the filter formats used by the node's fields,
please keep this in mind when assigning permissions to user roles.

Maintainer: Daniel Braksator (http://drupal.org/user/134005)
Project page: http://drupal.org/project/node_export.

Note: this module was originally built upon code from the node_clone module
maintained by Peter Wolanin (http://drupal.org/user/49851) at 
http://drupal.org/project/node_clone which was derived from code posted by
Steve Ringwood (http://drupal.org/user/12856) at 
http://drupal.org/node/73381#comment-137714


INSTALLATION
------------
1. Copy node_export folder to modules directory (usually sites/all/modules).
2. At admin/build/modules enable the Node export module in the Node export 
   package.
3. Enable any other modules in the Node export package that tickle your fancy.


CONFIGURATION
-------------
1. Enable permissions at admin/user/permissions.
   Security Warning: Users with the permission "use PHP to import nodes"
   will be able to change nodes as they see fit before an import, as well as 
   being able to execute PHP scripts on the server.  It is advisable not to
   give this permission to a typical node author, only the administrator or
   developer should use this feature.  You may even like to turn this module
   off when it is no longer required.
   This module does not check access to the filter formats used by the node's
   fields, please keep this in mind when assigning permissions to user roles.
2. Configure module at admin/settings/node_export.


USAGE
-----
1. To export nodes, either:
   a) Use the 'Node export' tab on a node page.
   b) Use the Content page (admin/content/node) to filter the nodes you wish to
      export and then choose 'Node export' under the 'Update options'.
   c) Use the VBO module: http://drupal.org/project/views_bulk_operations
   d) Use Drush: http://drupal.org/project/drush
2. To import nodes, either:
   a) Use the form at 'Node export: import' under 'Add content'
      (node/add/node_export).
   b) Use Drush: http://drupal.org/project/drush