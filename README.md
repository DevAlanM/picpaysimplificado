# Objetivo: PicPay Simplificado (Desafio OpenSource da empresa PicPay, realizado somente com foco em adquirir novos conhecimentos e desafios)
======================================================================================
## Temos 2 tipos de usuários, os comuns e lojistas, ambos têm carteira com dinheiro e realizam transferências entre eles. Vamos nos atentar somente ao fluxo de transferência entre dois usuários.
#
## Requisitos:
### 1 - Para ambos tipos de usuário, precisamos do Nome Completo, CPF, e-mail e Senha. CPF/CNPJ e e-mails devem ser únicos no sistema. Sendo assim, seu sistema deve permitir apenas um cadastro com o mesmo CPF ou endereço de e-mail.
### 2 - Usuários podem enviar dinheiro (efetuar transferência) para lojistas e entre usuários.
### 3 - Lojistas só recebem transferências, não enviam dinheiro para ninguém.
### 4 - Validar se o usuário tem saldo antes da transferência.
### 5 - Antes de finalizar a transferência, deve-se consultar um serviço autorizador externo, use este mock para simular (https://run.mocky.io/v3/8fafdd68-a090-496f-8c9a-3442cf30dae6).
### 6 - A operação de transferência deve ser uma transação (ou seja, revertida em qualquer caso de inconsistência) e o dinheiro deve voltar para a carteira do usuário que envia.
### 7 - No recebimento de pagamento, o usuário ou lojista precisa receber notificação (envio de email, sms) enviada por um serviço de terceiro e eventualmente este serviço pode estar indisponível/instável. Use este mock para simular o envio (http://o4d9z.mocklab.io/notify).
### 8 - Este serviço deve ser RESTFul.
=====================================================================================
#
## Stacks aprimoradas
### Utilizado Java Spring Boot com o Maven, H2 database, Tratamento de erros, pensamento lógico, estruturação de pastas e responsabilidades na API RestFull, Mapeamento, testes realizados no Postman
#
#### OBS: Ficou como obstáculo somente  a comunicação da notificação onde a url está indisponivel e ao referenciar a mesma ocorre um erro de timeout, tive que adaptar !!
