### Test Driven Development (TDD)

TDD é o desenvolvimento de software orientado a testes, Test Driven Development em inglês. Porém mais do que simplesmente testar seu código, TDD é uma filosofia, uma cultura. E foi fortemente adotado e influenciado pelo movimento ágil. Possui 3 grandes passos:
- Red: etapa inicial do TDD, onde você escreve um teste que falha, para alguma funcionalidade que você ainda vai escrever.
- Green: já com o teste criado, é o momento que você precisa fazer o teste passar, lembrando sempre de ir para solução mais simples primeiro.
- Refactor: etapa para eliminar códigos redundantes, remover acoplamentos e deixar o design de código mais legível.

### Por que poucos fazem TDD?

Existem alguns pontos principais que os desenvolvedores falam, quando tentam justificar porque não fazem TDD:

- Perda de tempo: os desenvolvedores acham que por ter de escrever além do código, os testes, vai fazer com que demorem mais para desenvolver. Para quê perder tempo aprendendo uma coisa que eu não vejo como útil/importante não é mesmo?
- Curva de aprendizado: o estilo de programar muda, é uma nova cultura e para isso, você precisa se adaptar. E é nesse ponto que a maioria desiste, pois não conseguem ver o valor do esforço inicial.

### O que ganho com TDD?

#### Reduz o tempo gasto em depuração e correção de bugs

Quando iniciamos o processo de correção de um bug, a primeira coisa que geralmente fazemos é tentar reproduzir o erro, para em seguida depurar o fluxo onde ocorre o bug para enfim analisar o estado dos objetos em busca da raíz do problema. Quando você não possui testes, você precisa mais uma vez realizar os passos de um teste funcional para depurar. Se você escrever um teste unitário que “estimule” o sistema a passar pelo código defeituoso, você estará “reproduzindo” o erro sem necessidade de executar a aplicação como um todo.

#### Não é desenvolvido código desnecessário

Essa pode parecer uma frase um pouco controversa, mas não é. Como o flow de desenvolvimento é "Criar testes antes, fazer solução depois", você acaba não criando código desnecessário, visto que você sempre faz o suficiente para os testes passarem.

#### Auxilia testes de regressão

É comum, ao corrigir um bug, introduzir um novo bug. Em outras palavras, a correção de um bug pode ter como efeito colateral que uma parte do software que antes funcionava deixe de funcionar. Quando isto ocorre, dizemos que o software regrediu. Chamam-se “teste de regressão” os testes que visam verificar a integridade geral do sistema quando um bug é corrigido, ou até mesmo quando uma nova funcionalidade é implementada no sistema. O uso do TDD vai reduzir a introdução de efeito colaterais junto com alterações no código. É claro que apenas na parte do código que seja coberta pelo testes unitários. Além disso, quando um teste passa a falhar após sua alteração, você acabou de identificar o bug num momento muito próximo de sua introdução.

#### Melhora a qualidade do código

O TDD encoraja que você pense antes de desenvolver a solução e que você sempre crie as soluções mais simples. Existe uma frase muito importante no TDD que é:

**"Se são necessárias muitas linhas de código criando objetos para uma simples asserção, então há algo de errado."**

#### Documentação pelos testes

Os testes nos ajudam a documentar o sistema se nomearmos ele bem. Como pensamos antes de codificar e fazemos testes pequenos para cada pedaço de funcionalidade, praticamente somos obrigados a escrever um teste legível. Se pararmos para ver todos os testes de uma funcionalidade temos ali praticamente uma documentação de caso de uso.

#### Refatoração constante

Como o próprio ciclo do TDD já sugere, a última etapa é a refatoração. Então, para cada teste que escrevemos, olhamos novamente nosso código e se nos sentirmos incomodados devemos refatorá-lo. O grande diferencial de trabalharmos com testes automatizados é que temos a segurança de fazer alterações, pois nossos testes devem garantir que nosso código continuará funcionando. Outro aspecto interessante é que refatorando a cada “verde”, evitamos que nosso código fique ilegível e com repetições desnecessárias.

### Tipos de testes

O TDD se baseia principalmente nos testes unitários, que de fato são a base para o desenvolvimento orientado por testes. Mas existem outros testes tão importantes quanto. Martin Fowler, que é basicamente um dos maiores apoiadores do TDD, disse o seguinte: a maioria do desenvolvimento sempre foi pensada na interface e, com isso, os testes mais criados também eram os de interface. Mas o problema é que esses testes são muito lentos e nós não queremos isso. Nós queremos respostas eficientes e rápidas, por isso, os testes unitários precisam ser o de maior de número e os mesmos precisam ser bem rápidos.

#### Teste Unitário (Unit Test)

O teste unitário tem por objetivo testar a menor parte testável do sistema (unidade), em geral, um método.

Idealmente, o teste unitário é independente de outros testes, validando assim cada parte ou funcionalidade individualmente.

#### Teste de fumaça (Smoke Test)

Esse é um teste pouco conhecido e pouco utilizado, mas que tem sua utilidade. Originado dos testes de hardware, ele serve para dizer somente se sua aplicação está respondendo corretamente ou não. Na nossa área de web, ele seria basicamente o teste de retorno das rotas e nada mais que isso.

#### Teste de Integração (Integration Test)

Teste de integração é a fase do teste de software em que módulos são combinados e testados em grupo. Ela vem depois dos testes unitários, em que os módulos são testados individualmente, e vem antes dos testes de aceitação, em que o sistema completo é testado num ambiente que simula o ambiente de produção.

O teste de integração é alimentado pelos módulos previamente testados individualmente pelos testes unitários, agrupando-os assim em componentes, como estipulado no plano de teste, e resulta num sistema integrado e preparado para o teste de sistema.

#### Teste de Aceitação (Acceptance Test)
O teste de aceitação verifica se todo o projeto funciona de acordo com sua especificação, ele já é um teste final, que visa juntar todos os módulos e testá-los em conjunto já a uma interface gráfica. Esses testes visam aferir se algo na interface faça o sistema não funcionar ou que dificulte o acesso ao usuário, um exemplo seria se um input não estivesse aparecendo para que dados fossem inseridos.