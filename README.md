# guia-wordpress
Anotações Wordpress

### Configuração LocalWP e VSCode
- Instalar, executar e configurar o WPLocal
  - https://localwp.com/
- Instalar plugin VSCode: `WordPress Snippets`
- Adicionar os arquivos estáticos (todo HTML) na pasta:
  `WPLocal\...\app\public\wp-content\themes\theme-example`

### Converter HTML p/ PHP
- Converter arquivo `index.html` p/ `index.php`
- Converter todos os arquivos `.HTML` p/ `.PHP`

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
- Nas páginas que necessitam deles, basta chamar a função abaixo:

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

### Inserir titulo da página dinamicamente
- Inserir a função abaixo dentro da tag `<title>`
```php
<?php bloginfo('name')?><?php wp_title('-')?>

// Exemplo:
<title><?php bloginfo('name')?><?php wp_title('-')?></title>
```

### Hierarquia de Modelos WordPress
- https://codex.wordpress.org/pt-br:Hierarquia_de_Modelos_WordPress
- https://codex.wordpress.org/images/0/02/Hierarquia_de_Arquivos_de_Tema_WordPress.png
