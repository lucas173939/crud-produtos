# CRUD de Produtos - Laravel

Este projeto é um **CRUD completo de produtos** desenvolvido com **Laravel 10** e **Bootstrap 5**.
Permite criar, listar, editar, visualizar e excluir produtos com interface amigável e validação de campos.

---

## Estrutura do projeto

```
app/
    Http/
        Controllers/
            ProductController.php
    Models/
        Product.php
resources/
    views/
        layouts/
            app.blade.php
        components/
            alert.blade.php
        products/
            index.blade.php
            create.blade.php
            edit.blade.php
            show.blade.php
            form.blade.php
routes/
    web.php
database/
    migrations/
    seeders/
```

---

## Requisitos

- PHP >= 8.1
- Laravel >= 10
- Composer
- MySQL ou MariaDB
- XAMPP (ou outro servidor local)

---

## Instalação

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/crud-produtos.git
cd crud-produtos
```

2. Instale as dependências PHP:

```bash
composer install
```

3. Instale dependências JS/CSS (opcional):

```bash
npm install
```

4. Configure o banco de dados no arquivo `.env`:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=crud_produtos
DB_USERNAME=root
DB_PASSWORD=
```

5. Crie o banco de dados no phpMyAdmin: `crud_produtos`

6. Rode as migrations:

```bash
php artisan migrate
```

7. Limpe cache do Laravel (opcional):

```bash
php artisan config:clear
php artisan cache:clear
php artisan route:clear
```

---

## Executar o projeto

Inicie o servidor:

```bash
php artisan serve
```

Abra no navegador:

```
http://127.0.0.1:8000/products
```

---

## Funcionalidades

- Criar produto → `products/create`
- Listar produtos → `products`
- Editar produto → `products/{id}/edit`
- Ver detalhes → `products/{id}`
- Excluir produto → botão "Excluir" na lista ou detalhes

- Validação de campos com mensagens de erro
- Layout responsivo usando Bootstrap
- Componentes reaproveitáveis (`alert`) para mensagens

---

## Observações

- Não suba o arquivo `.env` para o GitHub
- Para instalar em outro computador, rode `composer install` e `php artisan migrate`
- Pode customizar o layout adicionando CSS ou JS extras

---

## Autor

- Lucas Fernando

