# 0: Configura macOS para Desarrollo
## [Homebrew](https://brew.sh)
Homebrew es un 'package manager' (gestor de paquetes) que nos permite instalar, actualizar y eliminar aplicaciones en macOS más fácilmente
```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
Una vez instalado, ejecuta el siguiente comando para actualizar
```bash
brew update
```
## Programas
- Visual Studio Code
- Chrome/Firefox/Brave
- iTerm2
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
## Node.js
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
- Rectangle
- Docker
- Slack
- Postman
- Github Desktop
