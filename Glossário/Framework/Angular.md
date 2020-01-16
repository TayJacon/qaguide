### O Que é AngularJS?

O AngularJS é um framework de código aberto usado para construir aplicativos para web baseados em uma única página dinâmica. Os desenvolvedores também usam essa ferramenta para criar menus animados para páginas de internet baseadas em HTML.    

O AngularJS usa a arquitetura Model-View-Controller (MVC), que é usado no desenvolvimento de apps para a internet. Esse tipo de arquitetura consiste em:
- **Model** (Modelo) – a estrutura de dados que gerencia a informação e recebe comandos do controle.
- **View** (Visão) – a representação da informação.
- **Controller** (Controle) – responde aos comandos e interage com o modelo.

No contexto do AngularJS, o modelo é o framework, enquanto a visão é o HTML e o controle é o JavaScript. Assim, o AngularJS também pode ser chamado de framework Angular ou Angular Java. 

Descomplicando as coisas:
- O AngularJS combina JavaScript e HTML;
- O JavaScript aceita o comando do usuário e o envia para o AngularJS;
- O AngularJS usa o comando recebido para modificar o HTML.

### As Vantagens do AngularJS

O AngularJS é o queridinho dos desenvolvedores por algumas razões. São elas:
- **Combinação de Dados Bidirecional** – a arquitetura do AngularJS combina JavaScript e HTML, os códigos de ambos já estão sincronizados. Por isso, o framework poupa muito tempo dos desenvolvedores na hora da criação de aplicações e sites.
- **Diretivas** – O framework estende as funcionalidades do HTML com diretivas. Para ativar essas diretivas, os desenvolvedores adicionam o prefixo ng- nos atributos do HTML. Você pode acompanhar uma listagem de diretivas aqui. Abaixo está um exemplo do uso de diretivas.
```
<!DOCTYPE html>
<html>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
<body>
<div ng-app="" ng-init="age='20'">
<p>Input your age:</p>
<p>Age: <input type="text" ng-model="age"></p>
<p>You wrote: {{ age }}</p>
</div>
</body>
</html>
<!DOCTYPE html>
<html>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
<body>
<div ng-app="" ng-init="age='20'">
<p>Input your age:</p>
<p>Age: <input type="text" ng-model="age"></p>
<p>You wrote: {{ age }}</p>
</div>
</body>
</html>  
```
- **Estrutura do Código** – O AngularJS oferece códigos com templates, permitindo que você produza apps com códigos limpos. Isso não apenas economiza tempo, mas também torna mais fácil fazer qualquer modificação ou até mesmo corrigir uma aplicação.
- **Ambiente de Testes** – O framework tem suporte a Unit e testes integrados. 
- **Compatibilidade com Desktop e Mobile** –pode ser executado na maioria dos navegadores. E não apenas em computadores pessoais, mas também em dispositivos móveis. Flexibilidade e versatilidade são grandes características da ferramenta. 
- **Futuro Promissor** – O futuro do AngularJS é brilhante por conta da sua popularidade e funcionalidade. Sua base de usuários só está crescendo e ele tem ganhado cada vez mais documentos com tutoriais, que também têm recebido atualizações e ajudam novatos a se familiarizar com ele.  

### Antes de Aprender Sobre AngularJS

Antes de tudo, você precisa lembrar que o AnglarJS é um framework JavaScript. Consequentemente, é essencial saber o básico de programação da linguagem JavaScript antes de aprender qualquer coisa e a usar o AngularJS.

O mesmo se aplica a outras linguagens de programação, como HTML, CSS e Ajax. Conhecer a base do JavaScript antes de aprender sobre AngularJS permite que você:

- Se adapte ao rápido padrão de desenvolvimento do Angular;
- Saiba quando usar o framework;
- Se torne um desenvolvedor flexível e inovador.