### BDD (Behavior Driven Development)

Behavior Driven Development (BDD ou ainda uma tradução Desenvolvimento Guiado por Comportamento) é uma técnica de desenvolvimento Ágil que encoraja colaboração entre desenvolvedores, setores de qualidade e pessoas não-técnicas ou de negócios num projeto de software, relaciona-se com o conceito de verificação e validação. Foi originalmente concebido em resposta à Test Driven Development (Desenvolvimento Guiado por Testes), e tem se expandido bastante nos últimos anos.

Os focos do BDD são a linguagem e as interações usadas no processo de desenvolvimento de software. Desenvolvedores usam sua língua nativa em combinação com a linguagem ubíqua (ubiquitous language), que lhes permite concentrar nas razões pelas quais o código deve ser criado, e não em detalhes técnicos, além de minimizar traduções entre a linguagem técnica na qual o código é escrito e outras linguagens de domínio, usuários, clientes, gerência do projeto, etc.

### Práticas 

- Envolver as partes interessadas no processo através de Outside-in Development (Desenvolvimento de Fora para Dentro)
- Usar exemplos para descrever o comportamento de uma aplicação ou unidades de código
- Automatizar os exemplos para prover um feedback rápido e testes de regressão
- Usar deve (should em inglês) na hora de descrever o comportamento de software para ajudar esclarecer responsabilidades e permitir que funcionalidades do software sejam questionadas
- Usar simuladores de teste (mocks, stubs, fakes, dummies, spies) para auxiliar na colaboração entre módulos e códigos que ainda não foram escritos

### Cenários, ou Exemplos da Aplicação

Em BDD, um desenvolvedor, algum profissional do setor de qualidade ou até mesmo o cliente podem esclarecer os requisitos quebrando-os em exemplos específicos. Um exemplo de requisito de uma aplicação de vendas poderia ser: "Itens reembolsados ou substituídos devem ser retornados para o estoque". Esse requisito pode ser quebrado em dois exemplos de cenários, como:

***Cenário 1: Itens reembolsados devem retornar para o estoque***
- Dado que um cliente compra um jumper preto
- E eu tenho três jumper pretos no estoque
- Quando ele retorna com o jumper preto para reembolso
- Então eu devo ter quatro jumpers pretos no estoque

***Cenário 2: Itens substituídos devem ser retornados ao estoque***
- Dado que uma cliente compra um vestido azul
- E eu tenho dois vestidos azuis no estoque
- E eu tenho três vestidos pretos no estoque
- Quando ela retorna com o vestido para uma troca por um preto
- Então eu devo ter três vestidos azuis no estoque
- E dois vestidos pretos no estoque

Ao discutir os cenários os participantes se perguntam se a saída descrita sempre resulta daqueles eventos ocorridos no dado contexto. Isso ajuda a desvendar outros cenários e esclarecer os requisitos[4]. Por exemplo, um especialista do domínio pode notar que itens reembolsados não são sempre devolvidos ao estoque e então reorganizar os requisitos para algo do tipo "Itens reembolsados ou substituídos devem retornar ao estoque a não ser que estejam defeituosos". Este, por sua vez, ajuda os participantes a melhorar os requisitos, levando a uma melhor estimativa de quanto tempo aqueles requisitos levarão para serem implementados.

As palavras ***Dado que***, ***Quando*** e ***Então*** (Given, When e Then em inglês) são quase sempre usadas para guiar os cenários

#### Exemplos e Comportamento a nível de Unidad

Os mesmos princípios de exemplos, usando contextos, eventos e resultados podem ser usados para guiar o desenvolvimento a nível de unidade. Os exemplos seguintes descrevem um aspecto do comportamento de uma lista:

***Exemplo 1: Novas listas são vazias***
- Dado que uma nova lista é criada
- Então a lista deve estar vazia.

***Exemplo 2: Listas com alguma coisa dentro não podem estar vazias***
- Dado que uma nova lista é criada
- Quando eu adiciono um objeto a ela
- Então a lista não deve estar vazia

Ambos exemplos são necessários para descrever o comportamento do método esta Vazia de uma lista e obter os benefícios do mesmo. Estes exemplos podem ser automatizados utilizando até mesmo algum framework de TDD. Em BDD cada exemplo é comumente encapsulado num único método de teste, onde o nome do método é a descrição completa do comportamento. Por exemplo, usando Java e JUnit 4, os exemplos acima se tornariam:

```
public class ListaTest {

   @Test
   public void deveSaberSeEstaVazia() {
      Lista lista1 = new Lista();
      assertTrue(lista1.isEmpty());

      Lista lista2 = new Lista();
      lista2.adiciona(new Object());
      assertFalse(lista2.isEmpty());
   }
}
```

s vezes a diferença entre contexto, eventos e resultados pode ser mais explícita. Por exemplo:

```
public class ComportamentoDoControladorDeJanela {

    @Test
    public void deveFecharJanelas() {
        
        // Dado que
        ControladorDeJanela controlador = new ControladorDeJanela("Meu Quadro");
        Quadro quadro = new Quadro();
        
        // Quando
        controlador.fecharJanelas();
        
        // Então
        garantirQue(!quadro.estaAparecendo());
    }
}
```
