
Immob is a fast and lightweight Property Management System on top of [Symfony 5][1].

The user interface is built with [Bootstrap 4][2].



## Requirements

- PHP >= 7.3;
- PDO PHP Extension;
- GD PHP extension
- MySQL >= 5.7;
- And the [usual Symfony application requirements][3].

## Installation

1. Install Composer (see http://getcomposer.org/download)

2. Create new project via [Composer][4]

   ```
   $ composer create-project coderberg/residence-cms mywebsite.loc
   ```
3. Enter the newly created folder

   ```
   $ cd mywebsite.loc
   ```

4. After installing you should configure your web server's document / web root to be the ```public``` directory.

5. Create ```.env.local``` from ```.env``` file and fill in your database credentials

    ```
    DATABASE_URL=mysql://db_user:db_password@127.0.0.1:3306/db_name
    ```

6. Run

    ```
    $ php bin/console app:install
    ```

7. Go to http://mywebsite.loc/admin and log in.

   ```
   login: admin
   password: admin
   ```

8. To use feedback forms, configure MAILER_DSN in ```.env.local```

## Tests

1. Modify your DATABASE_URL config in ```.env.test.local```

   ```
   DATABASE_URL=mysql://db_user:db_password@127.0.0.1:3306/db_name
   ```

2. Execute this command to run tests:

   ```
   php bin/phpunit
   ```

## Additional documentation
-

[1]: https://symfony.com/
[2]: https://getbootstrap.com
[3]: https://symfony.com/doc/current/reference/requirements.html
[4]: https://getcomposer.org/doc/03-cli.md#create-project
[5]: https://github.com/Coderberg/ResidenceCMS/blob/master/docs/docker.md
