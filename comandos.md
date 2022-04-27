#Gerar imagem do projeto

```docker
docker build -t messiasdb1/eive-java-exam-4:prod .
```

#Configurar o postgres

```docker
docker pull postgres
```

```docker
docker run --name dbpetclinic -p 5432:5432 -e POSTGRES_DB=petclinic -e POSTGRES_PASSWORD=petclinic -e POSTGRES_USER=petclinic -d postgres
```

#Gerar contener do projeto

```docker
docker pull messiasdb1/eive-java-exam-4:prod
```

```docker
docker run --name petclinic -d -p 8080:8080 -e POSTGRES_URL=jdbc:postgresql://192.168.0.152:5432/petclinic -e POSTGRES_USER=petclinic -e POSTGRES_PASS=petclinic messiasdb1/eive-java-exam-4:prod
```