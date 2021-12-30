# guia-wordpress
Anotações Wordpress

- Instalar, executar e configurar o WPLocal
  - https://localwp.com/

- Instalar plugin VSCode: `WordPress Snippets`

- Adicionar os arquivos estáticos da página na pasta:
  `Ex: app\public\wp-content\themes\theme-ex`

- Converter arquivo `index.html` p/ `index.php`

- Criar o arquivo `style.css` na raíz do projeto com o conteúdo abaixo:

```css
/*
Theme Name: Nome do tema
Version: 1.0.0
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

- Criar header.php e footer.php
```php
// Header
<?php get_header();?>

// Footer
<?php get_footer();?>
```

#### Inserir barra do Wordpress

- Antes do fechamento da tag `</head>`
```php
<?php wp_head();?>
```

- Antes do fechamento da tag `</body>`
```php
<?php wp_footer();?>
```
