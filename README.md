FASE 1 – DOCUMENTAÇÃO + FRONTEND 

B) Melhorias do projeto
A versão inicial do projeto apresentava apenas dois campos: Nome e Email.
Foram adicionados novos campos e aprimorou-se a interface.

- Senha (para autenticação);
- Validação de CPF;
- Data de Nascimento;
- Telefone;
- Campos de cidade e estado;
- Sexo (seleção em lista suspensa);
- Layout mais moderno e responsivo;
- Formulário centralizado e com cores neutras;
- Botão de envio com destaque;
- Validação de campos obrigatórios;
- Mensagem de cadastro realizado com sucesso;
- Design moderno e responsivo.

C) Documentação do Sistema
Requisitos Funcionais
RF001: O sistema deve permitir o cadastro de novos usuários.
RF002: O sistema deve validar CPF e senha.
RF003: O sistema deve armazenar dados do usuário no banco.
RF004: O sistema deve garantir que o email seja único no cadastro.

Requisitos Não Funcionais
RNF001: O layout deve ser responsivo (ajustar-se a diferentes tamanhos de tela).
RNF002: A interface deve ser simples e intuitiva.
RNF003: O sistema deve ser desenvolvido com HTML, CSS e JavaScript (frontend).
RNF004: O tempo de resposta para ações deve ser inferior a 2 segundos.
RNF005: O backend deve utilizar Flask e SQLite

Diagrama Entidade Relacionamento
<img width="983" height="825" alt="Diagrama ER de banco de dados (pé de galinha)" src="https://github.com/user-attachments/assets/75abbdf8-44ec-4f15-ac04-a750f44fd867" />

 
Diagrama de Caso de Uso 
<img width="943" height="1070" alt="Diagrama de caso de uso (1)" src="https://github.com/user-attachments/assets/e1f04603-4337-4396-bf4e-76dc292f3ca7" />

FASE 2 – BACKEND + BANCO DE DADOS
a) Pesquisa sobre Flask e SQLite:
Flask é um microframework em Python voltado para criação de aplicações web rápidas e simples. 
SQLite é um banco de dados leve e embutido, ideal para protótipos e pequenos sistemas.

b) Fazer funcionar o sistema integrando o Backend ao BD
O backend será desenvolvido com Flask, criando rotas para inserção e listagem dos usuários. O banco SQLite armazenará os dados persistentes. A integração será feita via SQLAlchemy.

