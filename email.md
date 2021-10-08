

### Construa a estrutura do email

```
    $dadosEmail = array(
    'codigochamado => $codigoChamado,
    'titulo' => $request->titulo,
    'descricao' => $request->descricao,
    'datahora => $request->datahora,
);
```

### Chamar objeto Email passando o objeto dos dadosEmail

```
Mailt:to($request-.email->send(newCodigochamado($dadosEmail)));
```
### Importar Mailable



### A classe herda de Mailable
```
class CodigoChamado extends Mailable
```

### no constructor receber o array com metadados de email

```
public function __construct($dados)

```

### Chama o metodo markdown
```
this->markdown('emails.template-email-codigo-chamado)->subject('Codigo Chamado')
```


### Use o template do email

```
@component('mail::message')
# Introdution

@component('mail::button', ['url' => $url])
# Button 
@endcomponent

# Content
{{ config('app.name') }}
@endcomponent