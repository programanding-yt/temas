# 0: Configura macOS para Desarrollo
A continuación te presento una configuración sencilla para desarrollo web. Si bien, podrías utilizar únicamente la Terminal y cualquier navegador para empezar, te aseguro que estos programas harán más sencilla y grata tu experiencia. 
## [Homebrew](https://brew.sh)
Homebrew es un 'package manager' (gestor de paquetes) que nos permite instalar, actualizar y eliminar aplicaciones en macOS más fácilmente
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
Una vez instalado, ejecuta el siguiente comando para actualizar
```bash
brew update
```
## Programas
- [Visual Studio Code](https://code.visualstudio.com): IDE muy customizable y poderoso
- Chrome/Firefox/Brave: Te recomiendo instalar varios navegadores para probar tus aplicaciones web
- [iTerm2](https://www.iterm2.com): Terminal en esteroides 🦾
```bash
brew cask install \
 visual-studio-code \
 chrome \
 firefox \
 brave-browser \
 iterm2
```
## [Oh my zsh!](https://ohmyz.sh)
macOS Catalina utiliza zsh como Shell predeterminado , si utilizas una versión anterior, ejecuta el siguiente comando para installar zsh
```bash
brew install zsh
```
Instala Oh my zsh! para una configuración más amigable y productiva de zsh 
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
## [Node.js](https://nodejs.org/)
Node.js es un runtime de Javascript, nos permite ejecutar código JS sin necesidad de un navegador. Recomiendo utilizar Node Version Manager:
```bash
# Instalar nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.2/install.sh | bash
# Instalar node
nvm install node
```
Reinicia tu terminal y ejecuta el siguiente comando:
```bash
# Utilizar la versión de node que tengamos instalada
nvm use node
``` 
Para actualizar node:
```
nvm install node --reinstall-packages-from=node
```
Para ver las versiones de node disponibles:
```
nvm ls-remote
```
Para instalar una versión específica:
```
nvm install x.xx.xx
```
> Nota: la primera versión de node instalada por nvm se convierte en la versión predeterminada, para cambiarla utiliza:
```bash
nvm alias default x.xx.xx
``` 
## Opcionales
Estos programas no son fundamentales, pero los recomiendo ampliamente
- [Docker](https://www.docker.com/products/docker-desktop): gestor de Contenedores
- [Slack](https://slack.com): herramienta de comunicación colaborativa
- [Postman](https://www.postman.com): interacción con APIs 
- [Github Desktop](https://desktop.github.com): control de versiones de manera gráfica
- [Rectangle](https://rectangleapp.com): manejo de ventanas más sencillo
- [Flux](https://justgetflux.com/)
```bash
 brew cask install \
  rectangle \
  docker \
  slack \
  postman \
  github \
  flux
```
## Git
Asegúrate de configurar el archivo ~/.gitconfig, agregar tu información, y algunos atajos de los comandos más comunes. También puedes agregar tus propios atajos personalizados. Te dejo una lista con algunas sugerencias:
```bash
# Abrir el archivo '~/.gitconfig' en el editor Vim
vim ~/.gitconfig
```

```
[personal]
  name = Nombre Apellido
  email = tucorreo@correo.com
[github]
  user = usuario
[alias]
 a = add
 cm = commit -m
 s = status
 pom = push origin master
 pum = pull origin master
 co = checkout
 cob = checkout -b
 l = log
```
Para salir de Vim, presiona la tecla ```Esc``` y escribe ```:wq```, luego presiona Enter.
## Conclusión
¡Y eso es todo! Déjame en los comentarios cualquier pregunta o sugerencia, ¿qué programas utilizas tú para desarrollar?, ¿prefieres emacs, sublime text, atom, notepad++? Recuerda que todo es elección personal, experimenta con distintos programas, lo importante es tu comodidad.
¡Nos vemos en la próxima! 🌊🏄🏽‍♂️ 
