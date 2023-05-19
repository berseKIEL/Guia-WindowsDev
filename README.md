# Guia Entorno Desarrollo en Windows

Esta guía proporciona instrucciones paso a paso para configurar un entorno de desarrollo profesional para empezar como Web Developer en Windows utilizando WSL (Windows Subsystem for Linux) con la Distribución Ubuntu y otras herramientas como Windows Terminal, Microsoft PowerToys, Oh-My-Zsh, etc.

## Requisitos
- Windows 10 versión 2004 o posteriores
- Leer la guía oficial del<a href="https://learn.microsoft.com/es-es/windows/dev-environment/" target="_blank"> Entorno de Desarrollo en Windows </a>
- Eligir la distribución de Linux Ubuntu.

## Pasos de Configuración

- Instalar **Windows Terminal**, que está disponible en la <a href="https://aka.ms/terminal" target="_blank"> Microsoft Store</a>.
- Instalar **Windows PowerToys**, que está disponible en la <a href="https://aka.ms/installpowertoys" target="_blank">Microsoft Store</a>

### WSL
1. Abre desde tu Terminal PowerShell como Administrador y instala WSL con el siguiente comando:
```bash
wsl --install -d Ubuntu
```
2. Sigue los pasos que te indica WSL, estableciendo un usuario y una contraseña.
3. Actualiza los paquetes de distribución de Ubuntu y instala las herramientas necesarias como desarrollador
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install build-essential
```

### Editor de Codigo
1. Instala las paqueterias necesarias para utilizar WSL en VSCode:
```bash
sudo apt-get install wget ca-certificates
``` 
2. Descarga desde el sitio oficial de <a href="https://code.visualstudio.com/" target="_blank">Visual Studio Code</a> (VSCode).
3. Instala el paquete de extensiones de <a href="https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack" target="_blank">Desarrollo Remoto</a> en VSCode

### Oh my Zsh (opcional)
1. Leer la guia de <a href="https://github.com/ohmyzsh/ohmyzsh/wiki" target="_blank"> Oh My Zsh </a>

### Oh my Posh (opcional)
1. Leer la guia de <a href="https://ohmyposh.dev/docs/" target="_blank"> Oh my Posh </a>
