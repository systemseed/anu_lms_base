# Anu LMS

A Drupal recipe that sets up the basics of the Anu Learning Management System.

## Installation

If you are installing everything from scratch, we recommend [DDEV](https://ddev.com/) for
running Drupal and Anu LMS.

Skip step 1. if you have Drupal CMS or vanilla Drupal installed already.

1. Install Drupal CMS ([instructions](https://git.drupalcode.org/project/drupal_cms/-/wikis/Contributing-to-Drupal-CMS)).
   Installation on vanilla Drupal is also possible, but you have to
   additionally prepare Composer for recipe installation ([instructions](https://git.drupalcode.org/project/distributions_recipes/-/blob/1.0.x/docs/getting_started.md)).
2. Prepare Composer for Anu LMS installation:
   ```
   composer config allow-plugins.cweagans/composer-patches true
   composer require cweagans/composer-patches
   ```
3. Make sure you have Drush 13 or higher. Run this commands to check the version
   and upgrade Drush if needed:
   ```
   drush --version
   composer require drush/drush
   ```
4. Pull this recipe to your file system:
   ```
   composer require systemseed/anu_lms_base
   ```
5. Install the recipe:
   ```
   drush recipe recipes/anu_lms_base
   ```
6. Visit the [Anu LMS project page](https://www.drupal.org/project/anu_lms) for more information.
