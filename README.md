# lf
> * :memo: **Nueva configuracion**
## Administrador de archivos en terminal

**Repositorio OFICIAL:**  [lf](https://github.com/gokcehan/lf)
.
├── **nerd-font** [Fonts](https://www.nerdfonts.com/)
├── **Oh My Bash** [Script](https://ohmybash.nntoan.com/)
├── **Icons** [Search](https://www.nerdfonts.com/cheat-sheet)

**Nota:** Todo relacionado a este administrador de archivo en terminal lo puede encontrar en la pagina oficial, no es necesario reescribir todo la documentacion, por lo que solo me enfocare en las configuraciones basicas para manipular y entre otras funciones que estare integrando en el archivo de configuracion.

> :memo: **Note:** Esta configuracion solo esta enfocado para usuario Linux.
> #### Configuración 
>
> - Los archivos de configuración deben estar ubicado en el directorio de la instrucion para que funciones o puedes crear tu propia ruta siempre en tomar en cuenta la recomendación.
```bash
$ cd ~/.config/
```

## Instruciones
01. Crear directorio
```bash
mkdir -p ~/.local/bin
```
02. **Nota:** Descargar el binario LF.

**Tutorial OFICIAL:** [Config](https://github.com/gokcehan/lf/wiki/Tutorial)
```bash
curl -L https://github.com/gokcehan/lf/releases/latest/download/lf-linux-amd64.tar.gz | tar xzC ~/.local/bin
```

03. Crear enlace symbolico
```bash
ln -s ~/.local/bin/lf /usr/bin/lf
```

04. Descargar la configuracion desde github
```bash
git clone git@github.com:ISEATO-JR/lf.git ~/.config
```
Ejemplo de los archivos que usaremos:
```zsh

      $HOME~/.config/lf$ tree
      .
      ├── cleaner
      ├── icons
      ├── lfrc
      ├── LICENSE
      ├── opener
      ├── previewer
      └── README.mds
```
05.  Crear enlace symbolico de nuetra configuracion para poder usarlo desde la terminal.
```bash
ln -s ~/.config/lf/lfrc ~/.lfrc
```
Puede configurar los valores predeterminados de las siguientes variables para cambiar estas ubicaciones:
```bash
'$XDG_CONFIG_HOME ~/.config'
'$XDG_DATA_HOME ~/.local/share'
```
