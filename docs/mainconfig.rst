MainConfig
==========

This is suggested implementation of config files for yii projects, both new and existing.

Benefits
-------------
- These files are structured so that other configuration files are not accidentally edited. Think of it as "compartmentalized" configurations.
- Uses environment variables. No need to change "SERVER_MODE = production", the configuration will adapt to different environments


List of files
-------------

MainConfig.php
~~~~~~~~~~~~~~

Holds the core settings of the application.

behaviors.php
~~~~~~~~~~~~~

Add behaviors to be attached to the project ie. AjaxSendOptions

components.php
~~~~~~~~~~~~~~

Add components to be used via Yii::app()->componentName


imports.php
~~~~~~~~~~~

Add models to be imported on project initialization


modules.php
~~~~~~~~~~~

This is where you set or include new modules


params.php
~~~~~~~~~~

Setting of project wide variables via Yii::app()->params


routes.php
~~~~~~~~~~

Definition of url routes


Things to note
--------------

- You need to add this in your dev-servers

    * in /etc/sysconfig/httpd::

        # config for server mode (read by MainConfig.php)
        export SERVER_MODE=development

        # config for server master database (read by MainConfig.php)
        export MYSQL_MASTER_HOST=10.0.8.47
        export MYSQL_MASTER_USER=rarejob
        export MYSQL_MASTER_PASS=rarejob

        # config for server slave database (read by MainConfig.php)
        export MYSQL_SLAVE_HOST=10.0.8.48
        export MYSQL_SLAVE_USER=rarejob
        export MYSQL_SLAVE_PASS=rarejob

- On your local-pc, Rick have already set-up the necessary environment variables so no need to worry
- Environment variables are already set in staging servers
- On production servers, the config file is set to read common_ph/db/RJ_PDO.php settings instead
- Useable in backend servers
