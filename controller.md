### Redirecionamento

```
return redirect()->route('<path.view>'), [ <codigo> => $codigo ]

```

###  Consulta Chamado para edição posterior

```
function edit($codigo){

    $object = ClassObject.method($codigo);

    if ($object){
        $mensagens = Mensagem::where('id', 'chamado))->get();

        return veiw(<path.view>, compact('object', 'mensagens'));

    }else{
        return FacadesRedirect::back()->withErros(0).(['<messages>'])
    }
}

```