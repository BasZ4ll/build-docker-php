# build-docker-php
build-docker-php

#connect mysql php

create connect.php

```bash
<?php
$servername = "db";
$username = "root";
$password = "app";
 
try {
      $conn = new PDO(
        "mysql:host=$servername;dbname=student",
        $username, $password);
   
      // Set the PDO error mode
      // to exception
      $conn->setAttribute(PDO::ATTR_ERRMODE,
                  PDO::ERRMODE_EXCEPTION);
   
      echo "Connected successfully";
} catch(PDOException $e) {
      echo "Connection failed: "
        . $e->getMessage();
}
?>
```
#phpmyadmin
username : root
password : app
