### Usar form é obrigatorio o uso da tag

`@csrf`

### Tag para perocorre lista de objetos

```
foreach($blocos as $bloco)

<option value= {{bloco->id_bloco}}>

@endforeach
```


### Uso de jquery, para habilitacao interação do componentes dos formularios 

### Cria uma função customizada no controler do objeto e retonar um json


```public function pegarLocaisBloco($idBloco)

$locais = Local::where('id_bloco', $idBloco->get() );

return response()->json($locais);

```


### No jquery tratar o retorno da chamada como metodo assincrono



### Em seguida habilita o campo option


### Forçando os campos serem preenchidos

```
requet->validation(
     'field1' => 'required',
     'field2' => 'required',
     'field3' => 'required',
 )
```

`