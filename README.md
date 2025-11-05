# cadastro-WEB
Relatório

A função recebe uma string contendo um CPF (com ou sem pontos e traços), remove os caracteres especiais e realiza cálculos matemáticos para verificar se os dígitos verificadores (últimos dois números do CPF) estão corretos. Foi adicionado console.log(validarCPF) para testar a função e ver o resultado dela na tela útil para verificação rápida.

Objetivos:

Validar se um número de CPF informado é válido conforme as regras oficiais da Receita Federal do Brasil. Limpeza do CPF:
Remover qualquer caractere que não seja número (como “.” e “-”), garantindo que só restem dígitos. Validação de formato:
Verifica se o CPF tem exatamente 11 dígitos.
Impede CPFs com todos os dígitos iguais, como 11111111111, que são inválidos. Cálculo do primeiro dígito verificador:
Multiplica os nove primeiros dígitos por pesos decrescentes (10 a 2).
Calcula o resto da divisão (mod 11) para obter o primeiro dígito verificador.
Se o resto for 10 ou 11, o dígito é 0. Cálculo do segundo dígito verificador:
Usa agora os 10 primeiros dígitos (incluindo o primeiro dígito verificador).
Repete o processo anterior com pesos de 11 a 2.
O resultado é o segundo dígito verificador. Comparação final:
Compara os dígitos calculados com os dois últimos dígitos do CPF informado. Se ambos conferirem → CPF é válido
B) Melhorias do projeto:

A versão inicial do projeto apresentava apenas dois campos: Nome e Email. Foram adicionados novos campos e aprimorou-se a interface.

Senha (para autenticação);
Data de Nascimento;
Telefone;
Endereço;
Sexo (seleção em lista suspensa).
Layout mais moderno e responsivo;
Formulário centralizado e com cores neutras;
Botão de envio com destaque;
Validação de campos obrigatórios;
Mensagem de cadastro realizado com sucesso.

C) Documentação do Sistema:

Requisitos Funcionais:

RF001: O sistema deve permitir o cadastro de novos usuários.

RF002: O sistema deve validar os campos obrigatórios (nome, email e senha).

RF003: O sistema deve armazenar os dados em um banco de dados.

RF004: O sistema deve permitir a consulta dos usuários cadastrados.

RF005: O sistema deve permitir a atualização e exclusão de usuários.

RF006: O sistema deve garantir que o email seja único no cadastro.

Requisitos Não Funcionais

RNF001: O sistema deve ser acessível via navegador web.

RNF002: O layout deve ser responsivo (ajustar-se a diferentes tamanhos de tela).

RNF003: A interface deve ser simples e intuitiva.

RNF004: O sistema deve validar entradas de dados (ex: formato do email).

RNF005: O tempo de resposta para ações deve ser inferior a 2 segundos.

RNF006: O sistema deve armazenar as senhas de forma segura (criptografia).

Diagrama Entidade Relacionamento 
<img width="1366" height="768" alt="Imagem1" src="https://github.com/user-attachments/assets/ceb97420-f299-4f60-a703-2ab3b0b3331d" />


Diagrama de Caso de Uso 
<img width="1366" height="768" alt="Imagem2" src="https://github.com/user-attachments/assets/288e7a31-8e05-476c-8aff-65570ffd6b29" />
