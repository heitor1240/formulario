Js linha por linha:
Linha 1: Esta linha seleciona o elemento HTML com o ID 'cadastroForm' (o formulário) e adiciona um "event listener" para o evento submit. Isso significa que quando o formulário for enviado, a função fornecida será executada.
Linha 2: Impede que o comportamento padrão do evento de envio do formulário ocorra. No caso de um formulário, o comportamento padrão seria recarregar a página. preventDefault() previne isso.
Linha 3: Esta linha obtém o valor do campo de entrada (input) com o ID 'nome'. O valor inserido pelo usuário é armazenado na variável nome.
Linha 4: Similar à linha anterior, esta linha obtém o valor do campo de entrada com o ID 'email' e o armazena na variável email.
Linha 5: Esta linha seleciona o elemento da tabela com o ID 'tabelaCadastro', especificamente a primeira seção <tbody>. Isso permite que as linhas sejam adicionadas dinamicamente a essa seção da tabela.
Linha 6: Cria uma nova linha na tabela e a armazena na variável novaLinha.
Linha 7: Insere uma nova célula na primeira posição (índice 0) da linha recém-criada e a armazena na variável celulaNome.
Linha 8: Insere uma nova célula na segunda posição (índice 1) da linha recém-criada e a armazena na variável celulaEmail.
Linha 9: Define o conteúdo de texto da célula celulaNome com o valor armazenado na variável nome.
Linha 10: Define o conteúdo de texto da célula celulaEmail com o valor armazenado na variável email.
Linha 11: Reseta (limpa) o formulário após o envio, removendo os valores inseridos pelo usuário nos campos de entrada.
