### Customizar


### Customizando tb_blocos
```
class Bloco extends Model
{
    use HasFactory;
    protected $table = 'tb_blocos';
}

```
### Campos Obritagorios para modelo

```
protected $fillable = [

    'field1', 
    'field2',
    'field3,
]
```
