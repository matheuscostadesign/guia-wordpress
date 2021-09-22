# guia-wordpress
Anotações Wordpress

- Plugin VSCode: WordPress Snippets

- Adicionar os arquivos estáticos da página na pasta:

`Ex: app\public\wp-content\themes\theme-ex`

- Converter arquivo `index.html` p/ `index.php`

- Criar o arquivo `style.css` na raíz do projeto com o conteúdo abaixo:

```css
/*
Theme Name: Nome do tema
Theme URI: URL do projeto
Author: Nome do autor
Author URI: https://matheuscostadesign.github.io
Description: Descrição do tema
/*
```
- Criar o arquivo `screenshot.png` na raíz do projeto para servir como thumbnail do tema com o tamanho `880x660`

Inserir código PHP em todas URL/source

```php
<?php echo get_template_directory_uri() ?>/
```


 
