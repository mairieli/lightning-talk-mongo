# lightning talk: Iniciando com mongodb

#### Startando o mongo 
```bash
$ sudo systemctl start mongodb
```
#### Abrindo o mongo shell
```bash
$ mongo
```

#### Listar bancos
```
> show dbs
```

#### Usar/Criar um banco
```
> use <banco>
```

#### Listar coleções
```
> show collections
```

#### Usar/Criar uma coleção
```
> db.createCollection("colecao")
```

#### Inserindo documentos
```
> db.<colecao>.insertOne({dado: "dado"})
> db.<colecao>.insertMany([ {dado: "dado1"} , {dado: "dado2"} ])
```

#### Listando documentos
```
> db.<colecao>.find()
> db.<colecao>.find({dado: "dado2"})
```

#### Filtrando a listagem dos documentos
```
> db.<colecao>.find().sort({dado: 1})
> db.<colecao>.find().sort({dado: -1})
> db.<colecao>.find().limit(3)
> db.<colecao>.find({}, {dado: <0 ou 1>})
```
### Bibliotecas para o seu projeto!
 - [Mongolite](https://jeroen.github.io/mongolite/) (R)
 - [Jongo](http://jongo.org) (Java)
 - [Mongoose](http://mongoosejs.com) (Nodejs)
 - [PyMongo](https://github.com/mongodb/mongo-python-driver) (Python)
 
 
### Para conhecer mais recursos para o mongo acesse o link [awesome-mongodb](https://github.com/ramnes/awesome-mongodb)
