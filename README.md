# Reproduce issue 3351241

Issue: https://www.drupal.org/project/drupal/issues/3351241

```sh
ddev start
ddev composer install
ddev drush si --existing-config --account-pass="admin" --yes
```

Log in to [user/login](https://drupal-3351241.ddev.site/user/login) with username `admin` and password `admin`. Go to [node/add/article](https://drupal-3351241.ddev.site/node/add/article) and attempt to upload image to body field.

![Screenshot of body field](/web/modules/test_issue_3351241/screenshot.png "Screenshot of body field")
