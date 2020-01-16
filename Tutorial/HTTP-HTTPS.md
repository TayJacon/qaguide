## O que é HTTP?
HTTP são respostas padrões que os servidores enviam aos navegadores quando acessam um site. Estas respostas são códigos que ajudam a identificar o status de uma página na internet, e quando há um problema no site ou em algum recurso do site, que não permite que o mesmo seja carregado devidamente, temos um código que indica o erro, o HTTP Error.

HTTP significa HyperText Transfer Protocol (Protocolo de Transferência de Hipertexto). O HTTP é formado de um código de status e um motivo, que dá significado ao que o código representa.
## Então o que é HTTPS?
O HTTPS é “Protocolo de Transferência de Hipertexto” com Secure Sockets Layer (SSL), que é um certificado de segurança digital para fazer com que a troca de dados na internet seja mais segura.

Este certificado de segurança, o SSL, é apropriado para todos os websites, sendo indispensável para lojas virtuais, onde acontece troca de dados financeiros e de cartão de crédito, e qualquer outro site onde haja troca de dados pessoais como formulários cadastrais com nome, email, telefone e senhas.

Com o SSL a troca de dados entre o servidor e usuário é criptografada.

## Categorias do HTTP
Os códigos HTTP (ou HTTPS) tem três dígitos, sendo que o primeiro dígito do código significa a classificação dentro das cinco categorias.

1XX: Informativo – a solicitação foi aceita ou o processo continua em andamento;
2XX: Confirmação – a ação foi concluída ou entendida;
3XX: Redirecionamento – indica que algo mais precisa ser feito ou precisou ser feito para completar a solicitação;
4XX: Erro do cliente - indica que a solicitação não pode ser concluída ou contém a sintaxe incorreta;
5XX: Erro no servidor – o servidor falhou ao concluir a solicitação.

## Status-Code e Reason-Phrase
Traduzidos para o português estes termos significam código de status e frase razão, que são os elementos que compõe o HTTP.

Status-code são os três dígitos que indicam qual o erro para o servidor e navegador enquanto a frase razão é uma curta descrição do que este erro significa para melhor compreensão dos usuários.

Estes códigos e razões estão descritos na tabela abaixo para o seu conhecimento.

## Lista de Código de Status HTTP
Agora que você sabe o que é HTTP e HTTPS, confira essa lista com códigos HTTP, que tem os códigos mais comuns e outros que raramente são usados, baseado no W3.org.



| Código do Status HTTP | Significado do código HTTP | Significado do código HTTP |
| --- | --- | --- |
| 100 | Continue | Continuar |
| 101 | Switching Protocols | Mudando Protocolos |
| 102 | Processing | Processando |
| 200 | Ok | Ok |
| 201 | Created | Criado |
| 202 | Accepted | Aceito |
| 203 | Non-Authoritative Information | Não autorizado |
| 204 | No Content | Nenhum Conteúdo |
| 205 | Reset Content | Resetar Conteúdo |
| 206 | Partial Content | Conteúdo Parcial |
| 300 | Multiple Choices | Múltipla Escolha |
| 301 | Moved Permanently | Movido Permanentemente |
| 302 | Found | Encontrado |
| 303 | See Other | Veja outro |
| 304 | Not Modified | Não modificado |
| 305 | Use Proxy | Use Proxy |
| 306 | Proxy Switch | Proxy Trocado |
| 400 | Bad Request | Solicitação Inválida |
| 401 | Unauthorized | Não autorizado |
| 402 | Payment Required | Pagamento necessário |
| 403 | Forbidden | Proibido |
| 404 | Not Found | Não encontrado |
| 405 | Method Not Allowed | Método não permitido |
| 406 | Not Acceptable | Não aceito |
| 407 | Proxy Authentication Required | Autenticação de Proxy Necessária |
| 408 | Request Time-out | Tempo de solicitação esgotado |
| 409 | Conflict | Conflito |
| 410 | Gone | Perdido |
| 411 | Length Required | Duração necessária |
| 412 | Precondition Failed | Falha de pré-condição |
| 413 | Request Entity Too Large | Solicitação da entidade muito extensa |
| 414 | Request-URL Too Large | Solicitação de URL muito Longa |
| 416 | Request Range Not Satisfiable | Solicitação de faixa não satisfatória |
| 417 | Expectation Failed | Falha na expectativa |
| 500 | Internal Server Error | Erro do Servidor Interno |
| 501 | Not Implemented | Não implementado |
| 502 | Bad Gateway | Porta de entrada ruim |
| 503 | Service Unavailable | Serviço Indisponível |
| 504 | Gateway Time-out | Tempo limite da Porta de Entrada |
| 505 | HTTP Version Not Supported | Versão HTTP não suportada |

## O que é HTTP Error?

Error HTTP são os códigos HTTP que referem-se a erros de cliente e servidor, respectivamente, e impedem o carregamento de um site.

Quando você visita um site, o seu navegador faz uma solicitação ao servidor, e o servidor responde o navegador com um código, os códigos HTTP. São esses códigos que informam o que o servidor e navegador estão conversando entre si.

E com as informações do tópico anterior, fica fácil deduzir que os códigos HTTP Error são sempre começados pelos números 4 ou 5, que são respectivamente falhas do cliente (navegador) ou do servidor. Certo? Então vamos para o próximo passo.

## Quais os principais códigos de erro HTTP?

Conhecer os principais códigos de erro HTTP vai te ajudar a identificar problemas de navegação no seu site e minimizar os erros, além de entender a comunicação entre o seu navegador e o servidor do site que está tentando acessar.

Os principais códigos de erros HTTP que você deve ter em mente são os erros 403, 404, 500 e 503. Então veja agora o que significa e como corrigir os erros de HTTP mais comuns.

### Error 403
O Erro 403 – Forbidden é o erro “Proibido”. Isso significa que o servidor entendeu a solicitação do navegador mas se recusa a fazê-lo, pois o navegador não possui autorização para isso.

### Error 404
Quando você digita uma URL e recebe a mensagem ERROR 404 – PAGE NOT FOUND quer dizer que esta URL não te levou a lugar nenhum. Os motivos podem ser: a página não existe mais, a URL deste site mudou ou você digitou a URL errada.

### Error 500
Este erro não é tão comum de acontecer mas uma hora ou outra ele aparece! Erro 500 significa que algum script ou solicitação não foi compreendida – o que nem sempre indica um problema com o servidor. 

### Error 503
O status ERRO 503 significa serviço temporariamente indisponível. 