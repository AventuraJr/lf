#  <center>lf </center>
<p>Administrador de archivos de terminal</p>
<p>El código fuente se puede encontrar en el repositorio en https://github.com/gokcehan/lf</p>

<P> Todo relacionado a este administrador de archivo de terminal lo puede encontrar en la pagina oficial, no es necesario reescribir todo la documentacion, por lo que solo me enfocare en las configuraciones para que puedas manipular y entre otras funciones que estare integrando en el archivo de configuracion.</P>

> :memo: **Note:** Esta configuracion solo esta enfocado para usuario Linux.
> #### Configuracion 
>
> - Los archivos de configuración deben estar ubicado de archivo de configuracion del sistemas.      
      ```bash
            $ cd ~/.config/
      ```
Específico del usuario para todo el sistema operativo
# Instruciones
> :memo: **Nota** Clonar el repositorio con la jerarquia de configuracion previo
1. Ruta de directorio para clonar 

```bash
$ cd ~/.config/
```

2. Clear enlace simbolico suave
example
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
$ ln -s /etc/lf/lfrc ~/.config/lf/lfrc
$ ln -s /etc/lf/colors ~/.config/lf/colors
$ ln -s /etc/lf/icons ~/.config/lf/icons
$ ln -s ~/.local/share/lf/files
$ ln -s ~/.local/share/lf/marks
$ ln -s ~/.local/share/lf/tags
$ ln -s ~/.local/share/lf/history

```
Puede configurar los valores predeterminados de las siguientes variables para cambiar estas ubicaciones:
```bash
'$XDG_CONFIG_HOME ~/.config'
'$XDG_DATA_HOME ~/.local/share'
```
