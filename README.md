### Folder with a lot of projects

https://code.visualstudio.com/docs/setup/linux#_visual-studio-code-is-unable-to-watch-for-file-changes-in-this-large-workspace-error-enospc

```
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf
sudo sysctl -p
````

### Font fira code ubuntu

````
sudo apt install fonts-firacode
````

1. Open the command pallet with:
````
ctrl + shift + p
````
2. Search for “Preferences: Open Settings (JSON)” and open it.

3. Add the following lines in the file.
````
  "editor.fontFamily": "'Fira Code'",
  "editor.fontLigatures": true
 ````
4. Restart VSCode


### links
https://blog.theodo.com/2019/07/vscode-php-development/

### Solution on Linux for multiple laravel sail projects without install PHP in OS (docker)

Create a file named 'php' on /usr/local/bin: 
```
sudo touch /usr/local/bin/php
```

Make it executable: 
```
sudo chmod +x /usr/local/bin/php
```

Edit the file (with sudo) and paste this code:
```
path=$(printf '%s\n' "${PWD##*/}")
command="docker exec ${path}_laravel.test_1 php "$@""
echo "Running php on docker ${path}_laravel.test_1"
$command
```
--- 
```
command="docker exec php73nginx  php "$@""
echo "Running php on docker php73nginx"
$command
```
### phpcs
https://www.mclibre.org/consultar/php/otros/vsc-php-configuracion.html
https://marketplace.visualstudio.com/items?itemName=ikappas.phpcs
https://blog.theodo.com/2019/07/vscode-php-development/

### php debugger
https://blog.theodo.com/2019/07/vscode-php-development/
https://www.youtube.com/watch?v=LNIvugvmCyQ

### laravel artisan 
https://marketplace.visualstudio.com/items?itemName=ryannaddy.laravel-artisan

### plugin list

### NEEDED

* Auto Close Tag
* Auto Complete Tag
* Bracket Pair Colorizer
* Better PHPUnit (alt + T run | alt + G run previous) (https://marketplace.visualstudio.com/items?itemName=calebporzio.better-phpunit)
* Dotenv
* Docker
* Code Runner: ejecutrar trozo de código
* Favorites
* GitLens — Git supercharged
* Laravel Artisan
* Laravel Snippets
* Markdown Preview Enhanced
* Material Icon Theme
* PHP Debug
* PHP DocBlocker
* PHP Formatter
* PHP Namespace Resolver
* phpcs (Code Sniffer)
* Sublime Text Keymap and Settings Importer: OK (https://marketplace.visualstudio.com/items?itemName=ms-vscode.sublime-keybindings)
* Settings Sync (sync with github)
* TODO Highlight
* TODO Tree
* YAML

### NOT BAD NOT NEEDED

* advanced-new-file
* Bookmarks
* change-case: cambia el estil de las variables (camelCase, etc..)
* Color Highlight
* Git Blame
* Laravel Blade Spacer: 
* Markdown PDF: convert .md to .pdf
* Multiline Tricks
* Prettier - Code formatter (JavaScript|TypeScript|Flow|JSX|JSON|CSS|SCSS|Less|HTML|Vue|Angular|GraphQL|Markdown|YAML)
* Spanish Language Pack for Visual Studio Code
* 

### NOT NEEDED

* Angular v7 Snippets: NO
* Auto Import - ES6, TS, JSX, TSX: not needed
* Beautify: not needed
* Babel ES6/ES7: not needed
* Babel JavaScript: no needed
* Bootstrap 4, Font awesome 4, Font Awesome 5 Free & Pro snippets
* Code Spell Checker
* Docker Explorer
* ESLint
* Firebase
* Flow Language Support (javascript)
* HTML CSS Support
* HTML Snippets
* IntelliSense for CSS class names in HTML
* JavaScript (ES6) code snippets
* Live Server
* Node.js Modules Intellisense
* npm
* npm Intellisense
* Path Intellisense
* Paste JSON to Code
* Simple React Snippets
* SVG Viewer
* TypeScript Import
* TypeScript Importer
* Useful React Snippets
* vscode-pdf
* vscode-spotify
* Vscode Google Translate
* WakaTime


* Sublime Material Theme
* Terminal
* Useful React Snippets
* Vscode great icons
* vscode-icons

