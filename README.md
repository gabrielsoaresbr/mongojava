# Self study of MongoDB with Java, Spring Boot, Thymeleaf, Google Maps API, Materialize CSS

#### Preparing the development environment (Windows):
- Install MongoDB (msi installer)
- Configure envioriment viriable PATH with "C:\Program Files\MongoDB\Server\3.4\bin"
- Run MongoD (server): mongod --dbpath "c:\desenv\gabriel\mongodb" (in administration mode)
- Run Mongo and create a collection (client):
```
db.createCollection("alunos")
```
- Insert one:
```
db.alunos.insert({
    "nome": "Felipe",
    "data_nascimento": new Date(1994, 02, 26),
    "curso": {
        "nome": "Sistemas de informação"
    },
    "notas": [10.0, 9.0, 4.5],
    "habilidades": [{
        "nome": "inglês",
        "nível": "avançado"
    }, {
        "nome": "taekwondo",
        "nível": "básico"
    }]
})
```

- In the class MongojavaApplication, Run As Java Application ...
