
Getting Started  
---------------  
  
#### Via Cloning The Repository:  
  
  The easiest way to get started is to clone the repository:
  
```bash  
# Get the project  
git clone https://github.com/benakacha/cvtheque.git
```
  
#### Change directory  
```bash
cd cvtheque  
```

### Copy .env.dist to .env  
```
cp .env.dist .env  
```

#### Configure and add database credentials (in .env file)  

Open `.env` file and locate the database URL, then add your database credentials as shown here:

```
DATABASE_URL=mysql://db_user:db_password@127.0.0.1:3306/db_name
```

-   Change db_user to **YOUR_DATABASE_USERNAME**
-   Change db_password to **YOUR_DATABASE_PASSWORD**
-   db_name to **YOUR_DATABASE_NAME**
-   The database host by default is 127.0.0.1 and with a database port of 3306. You can leave this values as it is.
 
  
#### Install Composer dependencies  
```
$ composer install
```

#### Create Database

```bash
$ php bin/console doctrine:database:create
```

#### Update Schema

```bash
 $ php bin/console doctrine:schema:update --force
```

##### Run the application with

```bash
php bin/console server:run
```
