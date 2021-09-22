# guia-wordpress
Anotações Wordpress

- Instslar plugin VSCode: `WordPress Snippets`

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
- Criar o arquivo `screenshot.png` com as medidas `880x660px` na raíz do projeto para servir como thumbnail do tema

- Inserir função PHP antes do caminho dos arquivos em todas URL's

```php
<?php echo get_template_directory_uri() ?>/
```


 
