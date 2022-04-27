#  <center>lf </center>
<p>Administrador de archivos de terminal</p>
<p>El código fuente se puede encontrar en el repositorio en https://github.com/gokcehan/lf</p>

<P> Todo relacionado a este administrador de archivo de terminal lo puede encontrar en la pagina oficial, no es necesario reescribir todo la documentacion, por lo que solo me enfocare en las configuraciones para que puedas manipular y entre otras funciones que estare integrando en el archivo de configuracion.</P>

> :memo: **Note:** Esta configuracion solo esta enfocado para usuario Linux.
> #### Configuracion 
>
> - Los archivos de configuración deben estar ubicados en.      
      
Específico del usuario para todo el sistema operativo

 ```bash
 Unix '/etc/lf/lfrc ~/.config/lf/lfrc'
 ```
El archivo de colores debe estar ubicado en:
```bash
Unix '/etc/lf/lfrc ~/.config/lf/lfrc'
```
El archivo de iconos debe estar ubicado en:
```bash
Unix '/etc/lf/icons ~/.config/lf/icons'
```
El archivo de selección debe estar ubicado en:
```bash
Unix '~/.local/share/lf/files'
```
El archivo de marcas debe estar ubicado en:
```bash
Unix '~/.local/share/lf/marks'
```
El archivo de etiquetas debe estar ubicado en:
```bash
Unix '~/.local/share/lf/tags'
```

 El archivo de historial debe estar ubicado en:
```bash
Unix '~/.local/share/lf/history' 
```
Puede configurar los valores predeterminados de las siguientes variables para cambiar estas ubicaciones:
```bash
'$XDG_CONFIG_HOME ~/.config'
'$XDG_DATA_HOME ~/.local/share'
```
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