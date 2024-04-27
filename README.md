# MVC-Leonardo-Pedrosa
**Nome do Projeto:** Abandono Zero

**Descrição:** Pesquisa com o propósito de estabelecer um banco de dados contendo informações acerca dos principais motivos que levam ao abandono de cães.

**Arquitetura:** MVC (Model-View-Controller)

**Ferramenta de Diagramação:** Draw.io

**Modelos (Models):**
A entidade usuário está ligada ao login para que este possa ser verificado e posteriormente aprovado ou rejeitado.

&nbsp;&nbsp;&nbsp;&nbsp; As entidades Formulário Geral, Formulário Tem, Formulário não tem e Formulário Nulo são utilizadas para armazenar os dados fornecidos pelo usuário durante a pesquisa.

**Controladores (Controllers):**

- O controlador Login utiliza os métodos Validação e Autentificação para conferir as informações inseridas pelo usuário e o método redirecionar para enviar o usuário para o formulário 

- O controlador Dados utiliza os métodos listar e gravar para mostrar as informações do formulário e salvar os dados fornecidos pelos usuários 

**Views (Views):**
- O view homepage tem a função de apresentar todas as informações presentes na página inicial

- O view Tela login tem a função de apresentar todas as informações presentes na página de login

- Os views Formulário Geral, Formulário Tem, Formulário Quer Ter, Formulário Teve, Formulário Nulo servem para apresentar todas as informações presentes nos formulários

**Infraestrutura:**
A infraestrutura do projeto envolve um banco de dados relacional (MySQL ou PostgreSQL) integrado à arquitetura MVC através dos Models, responsáveis por interagir diretamente com o banco de dados para armazenar e recuperar dados dos formulários e usuários. Os Controllers, como Login e Dados, utilizam os Models para acessar e manipular esses dados. Além disso, podem ser integradas APIs externas para funcionalidades como autenticação e serviços relacionados ao abandono de animais. Outras dependências, como bibliotecas de validação e frameworks para gerenciamento de sessões, garantem a eficiência e segurança do sistema, seguindo uma abordagem modular e escalável para facilitar a manutenção e expansão do projeto.

**Implicações da Arquitetura:**

&nbsp;&nbsp;&nbsp;&nbsp; A arquitetura MVC é modular e separa as responsabilidades entre model, view e controller. Dessa forma, a escalabilidade do sistema se torna mais fácil, pois possibilita a adição ou modificação de funcionalidades sem afetar outras partes do código.

&nbsp;&nbsp;&nbsp;&nbsp; A separação da arquitetura em camadas torna a manutenção mais simples. Os Models representam a camada de dados e a lógica de negócios, permitindo reutilização e atualizações independentes. Os Controllers gerenciam o fluxo e a interação com o usuário, enquanto as Views se dedicam à apresentação dos dados, facilitando a manutenção e a resolução de problemas em partes específicas da aplicação.

&nbsp;&nbsp;&nbsp;&nbsp;A arquitetura MVC também favorece a testabilidade do sistema. Os Models encapsulam a lógica de negócios e a interação com o banco de dados, podendo ser testados de forma isolada (usando testes unitários, por exemplo) sem depender das Views ou Controllers. Os Controllers, que lidam com o fluxo de controle, podem ser testados com mocks ou stubs para simular a interação do usuário. As Views, embora sejam mais difíceis de serem testadas devido à sua natureza de apresentação, podem ser validadas visualmente ou por meio de testes de interface do usuário.

&nbsp;&nbsp;&nbsp;&nbsp; Outros aspectos importantes dessa arquitetura incluem os padrões de design e documentação. O uso da arquitetura MVC segue padrões comuns de design de software, tornando-o familiar para outros desenvolvedores e facilitando a colaboração em equipe. A estrutura organizada do MVC torna mais fácil para novos desenvolvedores entenderem e contribuírem para o projeto, pois as partes do sistema são claramente definidas e identificáveis.