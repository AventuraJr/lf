# lf
## Administrador de archivos en terminal

El código fuente lo puedes encontrar en el repositorio de [lf](https://github.com/gokcehan/lf)

**Nota:** Todo relacionado a este administrador de archivo en terminal lo puede encontrar en la pagina oficial, no es necesario reescribir todo la documentacion, por lo que solo me enfocare en las configuraciones basicas para manipular y entre otras funciones que estare integrando en el archivo de configuracion.

> :memo: **Note:** Esta configuracion solo esta enfocado para usuario Linux.
> #### Configuración 
>
> - Los archivos de configuración deben estar ubicado en el directorio de la instrucion para que funciones o puedes crear tu propia ruta siempre en tomar en cuenta la recomendación.
```bash
$ cd ~/.config/
```

## Instruciones
> :memo: **Nota:** Clonar el repositorio con la jerarquia de archivo que te agrego.
1. Ruta del directorio para clonar 

```bash
$ cd ~/.config/
```

2. Crear enlace simbolico suave
Ejemplo de los archivos que usaremos:
```zsh

      $HOME/.config/lf$ tree
      .
      ├── colors
      ├── file
      ├── history
      ├── icons
      ├── lfrc
      ├── LICENSE
      ├── marks
      ├── README.md
      └── tags
```
3. De esta forma crearemos los enlaces simbolico
```bash
$ ln -s ~/.config/lf/lfrc ~/.lfrc
$ ln -s /etc/lf/colors ~/.config/lf/colors
$ ln -s /etc/lf/icons ~/.config/lf/icons
$ ln -s ~/.local/share/lf/files
$ ln -s ~/.local/share/lf/marks
$ ln -s ~/.local/share/lf/tags
$ ln -s ~/.local/share/lf/history
$ set previewer ~/.config/lf/pv.sh
$ map i $~/.config/lf/pv.sh $f | less -R

```
Puede configurar los valores predeterminados de las siguientes variables para cambiar estas ubicaciones:
```bash
'$XDG_CONFIG_HOME ~/.config'
'$XDG_DATA_HOME ~/.local/share'
```
