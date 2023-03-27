# Docker Compose con Apache y PHP

### Ejecutamos el contenedor desde la imagen de docker hub que indicamos en el archivo docker-compose.yml
```
docker-composer up -d
```

### Para detener el contenedor
``` 
docker-composer down
```

Una diferencia importante entre docker-compose y docker run es que docker-compose recarga automaticamente todos losc cambios que se realicen en los archivos de la aplicacion, mientras que docker run no.