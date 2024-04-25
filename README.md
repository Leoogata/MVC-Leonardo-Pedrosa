# MVC-Leonardo-Pedrosa
Nome do Projeto: ## Abandono Zero

Descrição: Pesquisa com o propósito de estabelecer um banco de dados contendo informações acerca dos principais motivos que levam ao abandono de cães.

Arquitetura: MVC (Model-View-Controller)

Ferramenta de Diagramação: Draw.io

Modelos (Models):
A entidade usuário está ligada ao login para que este possa ser verificado e posteriormente aprovado ou rejeitado.

As entidades Formulário Geral, Formulário Tem, Formulário não tem e Formulário Nulo são utilizadas para armazenar os dados fornecidos pelo usuário durante a pesquisa.

Controladores (Controllers):
O controlador homepage utiliza os métodos Redirecionar e Listar para realizar as interações do usuário com a página inicial

O controlador Login utiliza os métodos Validação e Autentificação para conferir as informações inseridas pelo usuário e o método redirecionar para enviar o usuário para o formulário 

O controlador Dados utiliza os métodos listar e gravar para mostrar as informações do formulário e salvar os dados fornecidos pelos usuários 

Views (Views):
O view homepage tem a função de apresentar todas as informações presentes na página inicial

O view Tela login tem a função de apresentar todas as informações presentes na página de login

Os views Formulário Geral, Formulário Tem, Formulário Quer Ter, Formulário Teve, Formulário Nulo servem para apresentar todas as informações presentes nos formulários

Infraestrutura:
A infraestrutura do projeto envolve um banco de dados relacional (MySQL ou PostgreSQL) integrado à arquitetura MVC através dos Models, responsáveis por interagir diretamente com o banco de dados para armazenar e recuperar dados dos formulários e usuários. Os Controllers, como Login e Dados, utilizam os Models para acessar e manipular esses dados. Além disso, podem ser integradas APIs externas para funcionalidades como autenticação e serviços relacionados ao abandono de animais. Outras dependências, como bibliotecas de validação e frameworks para gerenciamento de sessões, garantem a eficiência e segurança do sistema, seguindo uma abordagem modular e escalável para facilitar a manutenção e expansão do projeto.

Implicações da Arquitetura:
Descreva as implicações da arquitetura em termos de escalabilidade, manutenção, testabilidade e outros aspectos importantes.