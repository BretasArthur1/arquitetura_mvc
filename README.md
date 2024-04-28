

# Nome do Projeto: Abandono 0

## Descrição
O projeto "Abandono 0", desenvolvido pelo INSPA, tem como objetivo entender as causas do abandono de animais. Utilizando um website interativo, coletamos informações de diversos perfis de usuários para elaborar relatórios que auxiliam pesquisadores a compreender e combater essa questão.

## Arquitetura: MVC (Model-View-Controller)
Este projeto adota a arquitetura MVC, que facilita a escalabilidade e a manutenção do código.

## Ferramenta de Diagramação
Utilizamos o draw.io para criar os diagramas da arquitetura do sistema.

### Modelos (Models)
- **Usuários**: Armazena dados dos usuários, incluindo ID, nome, email, senha e função (role).
- **Respostas de Formulário**: Contém as respostas submetidas pelos usuários, associadas a um ID de usuário e as respostas às perguntas específicas.
- **Relatórios**: Gera relatórios a partir dos dados coletados nos formulários, permitindo filtragem e análise detalhada.

### Controladores (Controllers)
- **Tutor**: Gerencia as operações de cadastro e login, incluindo a validação dos dados do usuário.
- **Admin**: Responsável por gerar, filtrar e baixar relatórios, além de gerenciar a dashboard.
- **Dashboard**: Permite aos administradores visualizar e interagir com o conjunto completo de dados e análises.

### Views (Views)
- **Home**: Página inicial do site, com informações gerais e acesso ao login/cadastro.
- **Formulários**: Telas de coleta de dados onde os usuários respondem perguntas relevantes.
- **Dashboard do Admin**: Interface onde os administradores acessam os relatórios e ferramentas de análise.

### Infraestrutura
- **Servidor**: Aplicação rodando em [especificar servidor], tratando das operações do lado do servidor.
- **Banco de Dados**: Usamos PostgreSQL para armazenar e gerenciar os dados coletados.

### Justifique as escolhas feitas e como elas impactam o projeto
Optamos pela arquitetura MVC devido à sua eficiência em separar a lógica do negócio da interface do usuário, o que facilita a manutenção e a expansão do projeto. A escolha do PostgreSQL foi devido à sua robustez e confiabilidade como SGBD.

#### Implicações da Arquitetura:
A arquitetura MVC possibilita uma melhor testabilidade e manutenção do código, além de permitir uma escalabilidade mais controlada. Cada componente pode ser desenvolvido e testado de forma independente, agilizando o processo de desenvolvimento.



