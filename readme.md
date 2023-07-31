Email Authentication using python package - django-use-email-as-username
Note: Dont run migrations after running django-admin startproject
1. Create superuse and delete it
2. Delete teh db.sqlite3 database
3. Comment out admin url
4. Comment out django.contrib.admin in settings.py
5. Add 'django_use_email_as_username.apps.DjangoUseEmailAsUsernameConfig', to Installed Apps
6. Run python manage.py create_custom_user_app
7. Add 'custom_user.apps.CustomUserConfig', to INSTALLED APPS
8. Add AUTH_USER_MODEL = 'custom_user.User' tp settings.py
9. Run makemigrations and migrate
10. Uncommnet django.contrib.admin and admin url
11. Run makemigrations and migrate again
12. 