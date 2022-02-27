# Linux

## Directorios
| Símbolo | Descripción |
| :-----------: | ----------- |
| `/` | El directorio raíz o superior. |
| `.` | El directorio actual. |
| `..` | El directorio superior, o padre, del directorio actual. |
| `~` | El directorio de trabajo del usuario. |


## Permisos
| Permiso | Octal | Binario | Archivo | Directorio | 
| :-----------: | :-----------: | :-----------: | ----------- | ----------- |
| `r` | 4 | 100 | Leer el contenido del archivo. | Listar el contenido del directorio. |
| `w` | 2 | 010 | Modificar/eliminar el archivo. | Crear/eliminar archivos. |
| `x` | 1 | 001 | Ejecutar el archivo. | Entrar en el directorio. |


## Descriptores de archivos
Son números enteros asociados con un archivo abierto o un flujo de datos. 

| Nombre | Descriptor | Abreviación |
| ----------- | :-----------: | :-----------: |
| Entrada estándar | 0 | stdin |
| Salida estándar | 1 | stdout |
| Error estándar | 2 | stderr |


## Redireccionamiento
| Símbolo | Descripción |
| :-----------: | ----------- |
| `>` | Redirecciona la salida estándar hacia un archivo: <ul><li>Si el archivo no existe, lo crea</li><li>Si el archivo existe, sobrescribe el contenido</li></ul> |
| `>>` | Agrega el contenido de la salida estándar a un archivo: <ul><li>Si el archivo no existe, lo crea</li></ul> |
| `2>` | Redirecciona el error estándar hacia un archivo: <ul><li>Si el archivo no existe, lo crea</li><li>Si el archivo existe, sobrescribe el contenido</li></ul> |
| `2>>` | Agrega el contenido del error estándar a un archivo: <ul><li>Si el archivo no existe, lo crea</li></ul> |
| `1>&2` | Redirecciona la salida estándar hacia donde apunta el error estándar. |
| `2>&1` | Redirecciona el error estándar hacia donde apunta la salida estándar. |
| <code>&#124;</code> | Utiliza la salida de un comando como entrada del siguiente. |


## PATH
PATH es una variable de entorno que le dice al shell en qué directorios buscar archivos ejecutables.

### Mostrar
```
$ echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/home/user/bin
```

### Modificar (temporal)
```
$ PATH="$PATH:/home/charlotte/bin"
$ export PATH
$ echo $PATH
/home/charlotte/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/home/user/bin
```

### Modificar (permanentemente)
```
$ echo 'export PATH="$PATH:/home/charlotte/bin"' | tee -a /home/charlotte/.bashrc
export PATH="$PATH:/home/charlotte/bin"
```

## Expansión de llaves (Brace Expansion)

### Ejemplo 01
```
$ echo 0{1,2,3}
01 02 03
```

### Ejemplo 02
```
$ echo {a..e}
a b c d e
```

### Ejemplo 03
```
$ echo {10..100..10}
10 20 30 40 50 60 70 80 90 100
```

### Ejemplo 04
```
$ echo {a..c}{1..3}
a1 a2 a3 b1 b2 b3 c1 c2 c3
```

### Ejemplo 05
```
$ echo {1,2{a..c},3}
1 2a 2b 2c 3
```
## Referencias
- [PATH Definition](http://www.linfo.org/path_env_var.html)
- [Viernes de Terminal: Bash [Expansión de Llaves]](https://blog.desdelinux.net/viernes-terminal-bash-expansion-llaves/)
