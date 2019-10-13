CRUD sem framework Responsivo e com Ajax.
=

**No banco de dados rodar:**

CREATE SCHEMA `estadao` DEFAULT CHARACTER SET utf8 ;

CREATE TABLE `estadao`.`carros` (`id` INT UNSIGNED NOT NULL AUTO_INCREMENT,`marca` VARCHAR(100) NOT NULL,`modelo` VARCHAR(100) NOT NULL,`ano` INT NOT NULL,`created_at` TIMESTAMP NOT NULL,PRIMARY KEY (`id`));

**Na raiz do projeto digitar o comando:**

php -S localhost:8000 -t public

**No navegador acessar:**

http://localhost:8000/view.php
