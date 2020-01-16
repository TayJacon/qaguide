### O Que PHP 7.4 Significa Para Você?

Para mais informações acesse o site do [php](https://www.php.net/manual/en/migration74.php).

#### Pré-carregamento

Vamos falar sobre código. Ao usar um framework ou bibliotecas, seus arquivos precisam ser carregados e vinculados a cada solicitação. O pré-carregamento é quando você pode carregar frameworks e bibliotecas no OPCache. Ele permite que o servidor carregue os arquivos PHP e os armazene na memória durante a inicialização e os disponibilize para solicitações futuras. É sobre fazer as coisas as coisas acontecerem rápido!

O pré-carregamento é executado por uma diretiva específica do php.ini: opache.preload. Este possui o compilador de scripts PHP e é executado quando o servidor é iniciado. Também pode ser usado para pré-carregar mais arquivos e escolher por incluí-los ou compilá-los.

Isso é impressionante. No entanto, se a origem dos arquivos pré-carregados for alterada, o servidor deverá ser reiniciado. Os arquivos pré-carregados também permanecem em cache na memória do OPCache para sempre.

No entanto, esses arquivos pré-carregados continuarão disponíveis para solicitações futuras, caso você precise usá-los novamente.

#### Spread Operator em Expressões de Array

Quando o PHP 5.6 foi lançado, o PHP começou a suportar argument unpacking (spread operator), mas agora, com a 7.4, podemos usar esse recurso com uma expressão de array. Argument unpacking é uma sintaxe para descompactar arrays e Traversables em listas de argument. E, para fazer isso, ele só precisa ser precedido por … (3 pontos). É isso.

Vamos conferir o exemplo:
```
$animals = ['dog', 'cat'];
$animalkingdom = ['lion', 'elephant', ...$animals, 'giraffe'];
// [‘lion’, ‘elephant’, ‘dog’, ‘cat’, ‘giraffe’];
```

#### Weak References

Agora, o PHP 7.4 tem uma classe Weak Reference, que não deve ser confundida com a classe WeakRed ou a extensão Weakref.

As WeakReferences permitem que o programador recupere uma reference a um object. Isso é útil porque não impede que o object seja destruído. Eles são úteis para implementar o cache como estruturas.

#### Typed Properties 2.0

Desde o PHP 5, type hints têm sido um recurso disponível, permitindo que você especifique o tipo de variável que se espera que seja passado para uma função ou classe. Nas migrações do PHP 7.2, a adição do object data type deu esperança de que houvesse mais disponíveis no futuro. O futuro é agora.

No novo 7.4, o PHP é capaz de suportar a seguinte lista de type:
```
bool, int, float, string, array, object, iterable, self, parent
any class or interface name
?type // where "type" may be any of the above
```

#### Arrow Functions 2.0

Funções anônimas (anonymous functions) no PHP tendem a ser longas e extensas, mesmo quando estão executando apenas operações simples.

Isso ocorre parcialmente devido a uma grande quantidade de clichê sintático e parcialmente devido à necessidade de importar manualmente as variáveis usadas.

Isso torna o código que usa closures simples confuso para ler e ainda mais difícil de entender.

Vamos dar uma olhada em um código que você usaria no PHP 7.3:
```
function array_values_from_keys($arr, $keys) {
    return array_map(function ($x) use ($arr) { return $arr[$x]; }, $keys);
}
```

Agora, aqui está a sintaxe mais concisa do PHP 7.4:

```
function array_values_from_keys($arr, $keys) {
    return array_map(fn($x) => $arr[$x], $keys);
}
```

Portanto, as arrow functions agora têm este formato simples:

```
fn(parameter_list) => expr
```

#### Descontinuações

Há muitas descontinuações acontecendo com a mudança para 7.4. A lista a seguir é uma breve visão geral das funções indicadas à descontinuação. Você pode encontrar uma explicação mais detalhada [aqui](https://wiki.php.net/rfc/deprecations_php_7_4):

- O tipo real 
- Magic quotes legacy
- array_key_exists() com objetos
- Filtro FILTER_SANITIZE_MAGIC_QUOTES 
- Métodos de reflexão export() 
- mb_strrpos() com codificação como 3rd argument
- Mix de ordem de parâmetro implode() 
- Desvincular $this de closures não estáticos 
- Função hebrevc()
- Função convert_cyr_string()
- Função  money_format()
- Função  ezmlm_hash()
- Função  restore_include_path()
- ini directiv allow_url_include