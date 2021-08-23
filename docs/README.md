## INSTALACION

### Instalar [Composer](https://getcomposer.org/)

En Arch Linux:

```bash
pacman -S composer
```

### Instalar laravel globalmente

```bash
composer global require laravel/install
```

Es necesario exportar el directorio de composer para poder utilizar los paquetes descargados directamente desde la linea de comandos.

```bash
export PATH="$HOME/.config/composer/vendor/bin:$PATH"
```

Se puede agregar esta linea al archivo `~/.bashrc` para que el directorio sea exportado automaticamente.

### Crear nuevo projecto

```bash
laravel new {project}"
```

Donde {project} es el nombre de nuestro nuevo proyecto.

Laravel permite inicializar un repositorio Git al momento de crear un nuevo proyecto.

```bash
laravel new {project} --git"
```

Tambien se puede utilizar la bandera --github para crear tanto un repositorio local como un repositorio remoto.

```bash
laravel new {project} --github="--public"
```

Nota: para poder utilizar esta bandera hay que contar con [GitHub CLI](https://cli.github.com/) instalado y configurado.

Una vez completada la instalacion se creara un nuevo directorio con el nombre {project}, que tendra la siguiente estructura.

```bash
.
|-- README.md
|-- app
|-- artisan
|-- bootstrap
|-- composer.json
|-- composer.lock
|-- config
|-- database
|-- package.json
|-- phpunit.xml
|-- public
|-- resources
|-- routes
|-- server.php
|-- storage
|-- tests
|-- vendor
`-- webpack.mix.js
```
