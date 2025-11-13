Introdução aos Códigos do Projeto: O projeto é uma aplicação web de Cadastro de Usuários desenvolvida seguindo uma arquitetura de pilha tecnológica moderna e leve, conforme especificado nos Requisitos Não Funcionais (RNFs).

Frontend (HTML, CSS e JavaScript): O frontend é responsável pela interface do usuário e pela validação inicial dos dados.

HTML: Define a estrutura do formulário de cadastro, incorporando todos os campos especificados (Nome, Email, Senha, CPF, Data de Nascimento, Telefone, Cidade/Estado, Sexo).

CSS: Aplica o estilo, garantindo um layout moderno e responsivo (RNF001) com um formulário centralizado e cores neutras.

JavaScript: Trata a interatividade e as validações de campos obrigatórios e de formato (como a Validação de CPF e a mensagem de sucesso), antes do envio dos dados para o backend.

Backend (Flask e Python): O backend é o coração da aplicação, responsável por processar as requisições, realizar validações complexas e interagir com o banco de dados.

Flask: Este microframework Python define as rotas que a aplicação usará. A principal rota será a de recebimento e processamento dos dados do formulário (POST).

Validações: O código do backend deve garantir as validações de CPF e Senha (RF002), além de assegurar que o Email seja único (RF004) antes de salvar.

SQLAlchemy: Atua como uma camada de Mapeamento Objeto-Relacional (ORM) para facilitar a comunicação entre o código Python e o banco de dados SQLite.

Banco de Dados (SQLite): O SQLite é o banco de dados leve e embutido (RNF005) usado para armazenar persistentemente os dados dos usuários (RF003).

FASE 1 – DOCUMENTAÇÃO + FRONTEND

B) Melhorias do projeto A versão inicial do projeto apresentava apenas dois campos: Nome e Email. Foram adicionados novos campos e aprimorou-se a interface.

Senha (para autenticação);
Validação de CPF;
Data de Nascimento;
Telefone;
Campos de cidade e estado;
Sexo (seleção em lista suspensa);
Layout mais moderno e responsivo;
Formulário centralizado e com cores neutras;
Botão de envio com destaque;
Validação de campos obrigatórios;
Mensagem de cadastro realizado com sucesso.
C) Documentação do Sistema Requisitos Funcionais RF001: O sistema deve permitir o cadastro de novos usuários. RF002: O sistema deve validar CPF e senha. RF003: O sistema deve armazenar dados do usuário no banco. RF004: O sistema deve garantir que o email seja único no cadastro.

Requisitos Não Funcionais RNF001: O layout deve ser responsivo (ajustar-se a diferentes tamanhos de tela). RNF002: A interface deve ser simples e intuitiva. RNF003: O sistema deve ser desenvolvido com HTML, CSS e JavaScript (frontend). RNF004: O tempo de resposta para ações deve ser inferior a 2 segundos. RNF005: O backend deve utilizar Flask e SQLite

Diagrama Entidade Relacionamento Diagrama ER de banco de dados (pé de galinha)

Diagrama de Caso de Uso Diagrama de caso de uso (1)

FASE 2 – BACKEND + BANCO DE DADOS a) Pesquisa sobre Flask e SQLite: Flask é um microframework em Python voltado para criação de aplicações web rápidas e simples. SQLite é um banco de dados leve e embutido, ideal para protótipos e pequenos sistemas.

b) Fazer funcionar o sistema integrando o Backend ao BD O backend será desenvolvido com Flask, criando rotas para inserção e listagem dos usuários. O banco SQLite armazenará os dados persistentes. A integração será feita via SQLAlchemy.

Relatório Final do Projeto:

Objetivos AtendidosO projeto alcançou seus principais objetivos, entregando um sistema funcional de cadastro que atende integralmente aos requisitos definidos:

Funcionalidade Principal (RF001): O cadastro de novos usuários foi implementado com sucesso.

Tecnologia (RNF003, RNF005): A aplicação foi desenvolvida usando a pilha tecnológica solicitada: HTML, CSS, JavaScript para o frontend e Flask com SQLite (via SQLAlchemy) para o backend e persistência de dados.

Usabilidade (RNF001, RNF002): A interface é intuitiva, moderna e totalmente responsiva, adaptando-se a diferentes dispositivos, o que melhora a experiência do usuário.

Integridade dos Dados (RF002, RF004): Foram implementadas validações cruciais no frontend e backend para garantir que apenas dados válidos (CPF, Senha) e únicos (Email) sejam armazenados.

Desafios Superados e Soluções

Desafio:Validação de CPF

Solução Implementada: Implementação de um algoritmo de verificação de dígitos no JavaScript (frontend) e uma revalidação de segurança no Flask (backend)

Requisito Atendido:(RF002)

Desafio:Layout Responsivo

Solução Implementada: Uso de Flexbox e/ou Grid Layout em CSS para garantir que o formulário e seus campos se ajustem perfeitamente a telas de desktop, tablet e mobile.

Requisito Atendido:(RNF001)

Desafio:Persistência de Dados

Solução Implementada: Utilização do SQLAlchemy para mapear a classe User (ou equivalente) no Python para a tabela no SQLite, simplificando as operações de inserção (RF003) e consulta (RF004).

Requisito Atendido:(RF003, RNF005 )

Próximos Passos (Sugestões de Evolução)

Para aprimorar o sistema, as seguintes funcionalidades poderiam ser consideradas:

Autenticação de Usuário: Implementar rotas de Login e Logout com gerenciamento de sessões.

Edição/Exclusão de Cadastro: Adicionar funcionalidades para que usuários logados possam editar ou excluir seus próprios dados.

Feedback em Tempo Real: Melhorar o feedback visual da validação de campos (por exemplo, indicando imediatamente se o CPF é inválido) para aprimorar o RNF004 (Tempo de Resposta).
