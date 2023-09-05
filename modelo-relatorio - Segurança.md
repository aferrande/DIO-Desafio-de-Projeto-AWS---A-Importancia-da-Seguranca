# RELATÓRIO DE IMPLEMENTAÇÃO DE MEDIDAS DE SEGURANÇA

Data: 04/09/2023
Empresa: Abstergo Industries 
Responsável: Arthur de Assis Ferrande

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Arthur de Assis Ferrande. O objetivo do projeto foi elencar medidas de segurança em conjunto dos serviços da AWS, com a finalidade de aumentar a segurança na empresa.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 medidas de segurança. A seguir, serão descritas as etapas da implementação:

Medida 1: 
- Utilizar o IAM para criação de usuários, grupos de usuários, roles, políticas, dentre outros. Não sendo mais necessário utilizar a conta root para realizar tarefas, facilita o gerenciamento e controle dos acessos, e aumenta a segurança de forma geral. Com o conceito de granularidade e do privilégio mínimo, evitamos que um usuário ou aplicação tenha acesso a algum recurso que não é necessário para efetuar suas atividades, nos protegendo de possíveis ações maliciosas, ou até mesmo erro humano. Podemos, por exemplo, retirar a permissão de uma role ou usuário de deletar/parar uma instância, assim garantindo maior controle sobre as funções e ações dentro das aplicações.
É importante também definir a necessidade de se criar uma senha forte para os usuários, que junto do MFA (Multi-Factor Authentication) adicionamos mais uma camada de segurança caso algum usuário perca sua senha ou tenha suas credenciais expostas ou roubadas. Outra prática interessante é colocar um tempo de expiração para credenciais e senhas.

Medida 2: 
- Utilizar criptografia e AWS Key Management Service para criação de chaves criptografadas para o acesso aos dados em repouso ou em trânsito contidos nos nossos banco de dados ou armazenamento. Evitando o risco desses dados serem acessados por pessoas não autorizadas.

Medida 3: 
- Podemos utilizar recursos como AWS WAF, AWS GuardDuty, dentre outros, para aumentar a segurança na rede das nossas aplicações. Protegendo de ataques e exploits, como desde um SQL injection à um brute force attack para roubo de informação.

Medida 4:
- Usar o Amazon Inspector para verificar possíveis vulnerabilidades e updates necessários nos nossos recursos, como por exemplo em um sistema operacional de uma instância EC2.

Medida 5:
- Utilizar o CloudWatch e CloudTrail para gerar logs e alarmes, assim conseguindo visualizar e gravar ações cometidas nas nossas aplicações. Esses logs são enviados para um bucket do S3, que também precisa ser seguro. Ou seja, acesso restrito e não público, e podemos adicionar a necessidade de MFA para deletar tal bucket.

## Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como esperado aumentar a segurança dos recursos e aplicações a ataques externos e acesso não autorizado, como a dos próprios usuários ao proteger suas credenciais de acesso. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos

https://aws.amazon.com/pt/products/security/  
https://docs.aws.amazon.com/iam/  
https://docs.aws.amazon.com/kms/  
https://docs.aws.amazon.com/guardduty/  
https://docs.aws.amazon.com/waf/  
https://aws.amazon.com/pt/inspector/  
https://aws.amazon.com/pt/cloudwatch/  
https://aws.amazon.com/pt/cloudtrail/  
https://aws.amazon.com/pt/s3/  

Assinatura do Responsável pelo Projeto:

Arthur de Assis Ferrande