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
```
