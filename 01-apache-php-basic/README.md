# Docker con Apache y PHP

### Construimos una imagen Docker a partir del Archivo Dockerfile el cual se encuentra en la ruta actual (.)
```
docker build -t "image_name" .
```

### Ejecutamos la imagen que acabamos de crear en el puerto 5000 de nuestra maquina, escuchara el puerto 80 del contenedor
```
docker run -p 5000:80 "image_name"
```

### Para correr la imagen en segundo plano
```
docker run -d -p 5000:80 "image_name"
```

### Para ver todos los contenedores activos
```
docker ps
```

### Para ver todos los contenedores
```
docker ps -a
```

### Para detener un contenedor
```
docker stop "container_id"
```

### Para eliminar un contenedor
```
docker rm "container_id"
```

## En caso de hacer cambios en el archivo index.php, estos cambios no se veran reflejados en el navegador, para esto debemos detener el contenedor, eliminarlo y volver a crearlo (crear otra vez la imagen y levantar un contendor con la nueva imagen)
