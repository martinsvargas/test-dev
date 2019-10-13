Instruçes para rodar o teste.
=

No banco de dados rodar:
-
CREATE SCHEMA `estadao` DEFAULT CHARACTER SET utf8 ;
CREATE TABLE `estadao`.`carros` (`id` INT UNSIGNED NOT NULL AUTO_INCREMENT,`marca` VARCHAR(100) NOT NULL,`modelo` VARCHAR(100) NOT NULL,`ano` INT NOT NULL,`created_at` TIMESTAMP NOT NULL,PRIMARY KEY (`id`));

Na raiz do projeto digitar o comando: 
-
php -S localhost:8000 -t public

No navegador acessar: 
-
http://localhost:8000/view.php




O teste
--------

### Back-End/PHP

A primeira etapa será o desenvolvimento **backend/PHP**:

**Descrição:**

- Você deverá desenvolver uma 'mini api' para que seja possível realizar operações CRUD do objeto Carro.
> **Obs:**
> - Você pode usar arquivo (txt, json) como banco de dados.
> - Cada carro deve ter ID, Marca, Modelo, Ano.

Sugerimos o retorno dessa 'mini api' nas seguinte urls:

 - `/carros` - [GET] deve retornar todos os carros cadastrados.
 - `/carros` - [POST] deve cadastrar um novo carro.
 - `/carros/{id}`[GET] deve retornar o carro com ID especificado.
 - `/carros/{id}`[PUT] deve atualizar os dados do carro com ID especificado.
 - `/carros/{id}`[DELETE] deve apagar o carro com ID especificado.

### Front-End

Para a segunda etapa do teste, você deverá desenvolver uma SPA (Single Page Application) e nela deve ser possível:

- Ver a lista de carros cadastrados
- Criar um novo carro
- Editar um carro existente
- Apagar um carro existente

> **Obs:**
> - A página deve ser responsiva.
> - A página deve funcionar 100% via AJAX, sem outros carregamentos de páginas.
> - Ao criar/editar um carro, o campo "marca" deverá ser um `SELECT`

### Observações importantes:

- Você não deve se prender aos arquivos do repositório. Fique a vontade para criar outros.
- Você pode usar frameworks, tanto para o front-end, quanto para o back-end, mas um código limpo será melhor avaliado.
- Você pode usar ferramentas de automação (Grunt, Gulp), mas deverá informar o uso completo para funcionamento do teste.
- Será considerado ponto positivo no teste a utilização de JS puro, orientação a objetos, design patterns e rotinas para testes.
- Será considerado ponto positivo o tempo gasto na realização do teste. Menos tempo e tudo funcionando conforme pedido será melhor avaliado.
