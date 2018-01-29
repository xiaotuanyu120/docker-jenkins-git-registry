## here we make nginx -> jenkins,git,registry

### env prepare
we need install docker and docker-compose, and start docker service

### first jenkins docker build need jdk8 file
1. pls download jdk8 here
2. pls extract it to jdk8 folder
3. pls tar and zip jdk8 to jdk8.tar.gz and move it to jenkins folder

### second boot up nginx gitlab jenkins registry by using docker-compose
``` bash
docker-compose -f docker-compose-prod.yaml up -d
```
> also you can use the separate yaml file to boot up them separately
