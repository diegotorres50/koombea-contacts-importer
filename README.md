<p align="center"><a href="https://www.koombea.com/" target="_blank"><img src="https://www.koombea.com/wp-content/uploads/2020/04/Logo-with-solid-background.jpg"></a></p>

## Koombea Challenge - Contact Importer with Laravel by Diego Torres 👋

This is a technical test to import contacts keeping in mind some rules that you may read [here](RFC.md).

On the other hand, you may be interested to try this demo out, so feel free to do it here: http://contacts-manager-freelancercontracts166926.codeanyapp.com/ 

## What you are going to get

![preview.png](preview.png)

This is the prototype preview of contact importer developed with Laravel 8 in PHP.


## Do you need to run it locally?

PHP, MYSQL & Apache or Nginx server are required.

To run this demo in your local environment, please keep in mind the next.

- Create a database locally named koombea utf8_general_ci
- Download composer https://getcomposer.org/download/

- Clone this repository

    ![clone_repo.png](clone_repo.png)

- Open the console and cd your project root directory
- Run 
    ```composer install or php composer.phar install```

    ![composer_install.png](composer_install.png)

- Run 
    ```php artisan key:generate```

    ![php_artisan_key.png](php_artisan_key.png)

- Rename the file .env.example to .env in project root and make sure to set the right and existing database name as shown below

    ![env_config.png](env_config.png)

- Run 
    ```php artisan migrate```

    ![php_artisan_migrate.png](php_artisan_migrate.png)

- Run 
    ```php artisan serve```

    ![php_artisan_serve.png](php_artisan_serve.png)
    
**And Bingo!!!**

![preview_login.png](preview_login.png)

if you are going to import large files with many records, i suggest to run queues, like so:

```php artisan queue:work```

![php_artisan_queue.png](php_artisan_queue.png)


## How to use it

#### You need to be autheticated

![login_zone.png](login_zone.png)

You may use next credentials to log in application:

    - User: koombea2@koombea.co
    - Pass: 12345678

However, i recommend to register your user:

![register.png](register.png)


#### Import your contacts

![documents.png](documents.png)

Once logged, you may click on Contact list button

![importing.png](importing.png)

Pickup a CSV format file (separated values by semicolon ";") with click on Browse button and finally click on Upload button as shown above. 


#### View importing history

![imported_files.png](imported_files.png)

To see importing files history, you may click on Import Contacts


#### Monitor errors

![invalid_imports.png](invalid_imports.png)

In case you got errors while importing files, you may click on Errors button to see a log.


## Author

👤 **Diego Torres**

- Linkedin: [https://www.linkedin.com/in/diegotorrescampuzano/](https://www.linkedin.com/in/diegotorrescampuzano/)

---

_Thanks so much Koombea ❤️_
