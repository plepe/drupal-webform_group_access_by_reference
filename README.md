# Webform Group Access by Reference
This module restricts access to webform submissions based on group membership
(resp. role) referenced by a field of the webform.

## INSTALLATION
```sh
composer require drupal/webform_group_access_by_reference
drush pm:install webform_group_access_by_reference
```

## HOW TO USE
1. Create a Webform
2. Add a field of type "Entity select" or similar (currently, only single value elements are supported). Make the field reference Groups.
3. Go to the Settings of a webform (`admin/structure/webform/manage/mywebform/settings`). You'll find a "Settings of third parties" box, with the Settings of "Webform Group Access by Reference`.
  * In "Group Reference Field" enter the key of the field you just added.
  * Optionally, you can enter the key of a group role in "Required Role in Group".

## CONTRIBUTORS
* Stephan Bösch-Plepelits <skunk@xover.mud.at>
