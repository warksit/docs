## Automatic Installation

Note: if you face any problem in any of the steps you should report it at [github](https://github.com/serverfireteam/panel/issues/new)

1. First you need to create a laravel 5.2 or 5.1 or 5.0  project.

2. Add LaravelPanel with runing this code in CMD 
    ```
        composer require serverfireteam/panel
    ```
    Or Add the package to require section of composer And run the composer update command, the package and its dependencies     will be installed.
    Laravel 5.2 :
    ```json
    {
        "require": {
            "serverfireteam/panel": "1.4.*"
        },
    }
    ```    
    Laravel 5.1 :
    ```json
    {
        "require": {
            "serverfireteam/panel": "1.3.*"
        },
    }
    ```
    Laravel 5.0 :
    ```json
    {
        "require": {
            "serverfireteam/panel": "1.2.*"
        },
    }
    ```


3. Add the ServiceProvider of the package to the list of providers in the config/app.php file

    laravel 5.1 and laravel 5.2
    ```php
    'providers' => array(
        Serverfireteam\Panel\PanelServiceProvider::class
    )
    ```
    laravel 5.0
    ```php
    'providers' => array(
        'Serverfireteam\Panel\PanelServiceProvider'
    )
    ```

4. Run the following command in order to publish configs, views and assets.

    ```bash
    php artisan panel:install

    ```

5. Go to your domain.com/panel and you can login with the following username and password :

    user : admin@change.me

    password : 12345



[>Next (Make crud with crud commands) ](/docs/master/crud-commands)
