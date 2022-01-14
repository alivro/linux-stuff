# Docker

## Comandos

### docker images
Lista las imágenes:
```
docker images [OPTIONS] [REPOSITORY[:TAG]]
```

#### Opciones
| Nombre | Abreviatura  | Descripción |
| ----------- | ----------- | ----------- |
| `--all` | `-a` 	| Muestra todas las imágenes (por defecto oculta las imágenes intermedias). |
| `--quiet` | `-q` 	| Solo muestra los IDs de las imágenes. |


### docker ps
Lista los contenedores:
```
docker ps [OPTIONS]
```

#### Opciones
| Nombre | Abreviatura  | Descripción |
| ----------- | ----------- | ----------- |
| `--all` | `-a` | Muestra todos los contenedores (por defecto solo muestra los que están en ejecución). |
| `--last` | `-n` | Muestra los últimos n contenedores creados (incluye todos los estados).  |
| `--latest` | `-l` | Muestra el último contenedor creado (incluye todos los estados).  |
| `--quiet` | `-q` 	| Solo muestra los IDs de los contenedores. |


### docker pull
Descarga una imagen de un repositorio o registro:
```
docker pull [OPTIONS] NAME[:TAG|@DIGEST]
```

#### Opciones
| Nombre | Abreviatura  | Descripción |
| ----------- | ----------- | ----------- |
| `--all-tags` | `-a` | Descargar todas las imágenes etiquetadas en el repositorio. |


### docker restart
Reinicia uno o más contenedores:
```
docker restart [OPTIONS] CONTAINER [CONTAINER...]
```


### docker rm
Elimina uno o más contenedores:
```
docker rm [OPTIONS] CONTAINER [CONTAINER...]
```

#### Opciones
| Nombre | Abreviatura  | Descripción |
| ----------- | ----------- | ----------- |
| `--force` | `-f` | Fuerza la eliminación de un contenedor en ejecución (SIGKILL). |


### docker rmi
Elimina uno o más imágenes:
```
docker rmi [OPTIONS] IMAGE [IMAGE...]
```

#### Opciones
| Nombre | abreviatura  | Descripción |
| ----------- | ----------- | ----------- |
| `--force` | `-f` | Fuerza la eliminación de la imagen. |


### docker run
Ejecuta un comando en un nuevo contenedor:
```
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```

#### Opciones
| Nombre | abreviatura  | Descripción |
| ----------- | ----------- | ----------- |
| `--detach` | `-d` | Ejecuta un conteneder en segundo plano e imprime su ID. |
| `--hostname` | `-h` | Nombre de host del contenedor. |
| `--name` | | Asigna un nombre al contenedor. |
| `--workdir` | `-w` | Directorio de trabajo dentro del contenedor. |


### docker start
Inicia uno o más contenedores detenidos :
```
docker start [OPTIONS] CONTAINER [CONTAINER...]
```


### docker stop
Detiene uno o más contenedores en ejecución :
```
docker stop [OPTIONS] CONTAINER [CONTAINER...]
```


### docker version
Muestra información sobre la versión de Docker:
```
docker version [OPTIONS]
```

## Referencias
- [docker](https://docs.docker.com/engine/reference/commandline/docker/)
