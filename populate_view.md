

### Popular
```
public function create(){
    $blocos = Bloco::get();
    $locais = Local::get();
    tipos = Tipo:get();
    $categorias = Categoria:get();

    return view('chamados.criacao', compact('blocos', 'locais', 'tipos', 'categorias'))
}

```