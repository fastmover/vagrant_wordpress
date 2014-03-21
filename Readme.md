#Vagrant box with Wordpress ready to install via: Composer

    vagrant up
    
    vagrant ssh
    
    cd /var/www
    
    composer install
    
From here you can run the wordpress install using mysql database:

    Username: root
    Password:
    Database: database
    host: localhost
    

You'll also want to copy the .htaccess and index.php files from the public/wp directory to the public directory.  Modify the index.php:

    require( dirname( __FILE__ ) . '/wp/wp-blog-header.php' );
