# guia-wordpress
Anotações Wordpress

### Configuração LocalWP e VSCode
- Instalar, executar e configurar o WPLocal
  - https://localwp.com/
- Instalar plugin VSCode: `WordPress Snippets`
- Adicionar os arquivos estáticos da página na pasta:
  `Ex: app\public\wp-content\themes\theme-ex`

### Converter HTML p/ PHP
- Converter arquivo `index.html` p/ `index.php`

### Configurando tema
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

### Thumbnail do tema
- Criar o arquivo `screenshot.png` com as medidas `880x660px` 
- Inserir a imagem na raíz do projeto para servir como thumbnail do tema
- Ativar o novo tema no painel do Wordpress e excluir os demais

### Ajustar diretórios
- Inserir função PHP antes do caminho dos arquivos em todas URL's do site
- Arquivos CSS, imagens, scripts, etc

```php
<?php echo get_template_directory_uri() ?>/

// Exemplo arquivo CSS:
<link rel="stylesheet" href="<?php echo get_template_directory_uri() ?>/css/main.min.css">
```

### Componentes que se repetem: Header e Footer
- Criar os arquivos: `header.php` e `footer.php` 
- Inserir a estrutura HTML nesses arquivos
- Nas páginas que necessitam deles, basta inserir os comando abaixo:

```php
// Header
<?php get_header();?>

// Footer
<?php get_footer();?>
```

### Inserir barra do Wordpress

```php
// Antes do fechamento da tag `</head>`
<?php wp_head();?>

// Antes do fechamento da tag `</body>`
<?php wp_footer();?>
```
