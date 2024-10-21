//index.html linha por linha:

Na seção `<head>`, são definidos alguns detalhes importantes da página, como a codificação de caracteres UTF-8 e as configurações de viewport. Isso é bem legal porque ajuda a garantir que a página fique bonita em diferentes tamanhos de tela. O título da página é "Cadastro", e um arquivo CSS chamado `style.css` é vinculado para dar um visual bacana à página. 

No `<body>`, a estrutura começa com uma `<div>` que tem a classe `container`. Essa `<div>` serve para organizar tudo que está dentro dela. Logo de cara, temos um cabeçalho de nível 1 que mostra o título "Formulário de Cadastro". Depois, vem o formulário com o ID `cadastro`, que contém dois campos: um para o nome, que é do tipo texto, e outro para o email, que é do tipo email. Ambos têm texto de sugestão e são obrigatórios, então não dá pra esquecer de preencher. E para finalizar, temos um botão que diz "Cadastrar".

Abaixo do formulário, há uma tabela com o ID `tabelaCadastro`, que vai exibir os dados dos usuários cadastrados. A tabela tem um cabeçalho com duas colunas: "Nome" e "Email". O corpo da tabela começa vazio porque os dados vão ser adicionados aos poucos. Por último, um arquivo JavaScript chamado `script.js` é vinculado, e isso permite que a gente coloque a lógica para fazer o formulário e a tabela funcionarem juntos. A estrutura termina com as seções `<body>` e `<html>`.


//style.css linha por linha:

O código CSS começa definindo as regras para o corpo da página. Aqui, a fonte é configurada para ser a Arial, mas também pode usar uma fonte sans-serif se não tiver. O fundo da página é um cinza claro (`#f4f4f4`), e as margens e o preenchimento do corpo estão zerados, então não aparece nenhum espaço estranho ao redor do conteúdo.

Depois, a classe `.container` é estilizada para centralizar a área na página. A largura da `.container` é de 50% da tela, e as margens são automáticas, ajudando a centralizar tudo. Um espaço interno de 20 pixels é adicionado para dar um respiro, e o fundo é branco. As bordas são arredondadas com um raio de 5 pixels, e tem uma sombra suave para dar uma sensação de profundidade.

O título da página, que está em `<h1>`, é centralizado com a regra `text-align: center;`, o que faz o texto ficar bem no meio.

O formulário é estilizado para ser um contêiner flexível usando `display: flex`, o que organiza os campos de entrada em uma coluna. Isso faz com que cada elemento do formulário fique um embaixo do outro.

Os campos de entrada (`<input>`) têm uma margem de 10 pixels embaixo para separar um do outro. Eles também têm um preenchimento de 10 pixels, o que dá um espaço confortável dentro. As bordas são de um cinza claro (`#ccc`) e arredondadas em 5 pixels.

O botão de envio tem 10 pixels de preenchimento e um fundo verde (`#28a745`). O texto do botão é branco, e ele não tem bordas, mantendo as bordas arredondadas em 5 pixels. Quando o mouse passa por cima do botão, ele muda para um verde um pouco mais escuro (`#218838`), dando um feedback visual que é bem legal.

As regras para a tabela começam definindo que ela vai ter 100% da largura disponível e uma margem em cima de 20 pixels. A propriedade `border-collapse: collapse;` é usada para tirar o espaço entre as bordas das células da tabela.

As células de cabeçalho (`<th>`) e as de dados (`<td>`) têm 10 pixels de preenchimento e são alinhadas à esquerda. As bordas de ambas são sólidas e cinza claro (`#ddd`).

Por fim, a parte de cabeçalho da tabela (`<thead>`) é estilizada com um fundo cinza muito claro (`#f8f9fa`), o que dá um contraste legal com o resto da tabela.


//script.js linha por linha:

Esse código JavaScript tem a missão de gerenciar o envio do formulário de cadastro de usuários e mostrar as informações em uma tabela. Tudo começa com a adição de um ouvinte de eventos ao formulário que tem o ID `cadastroForm`. Quando alguém envia o formulário, uma função anônima é acionada.

Dentro dessa função, a primeira coisa que acontece é chamar `event.preventDefault()`. Isso serve para evitar que o formulário faça o que normalmente faz, ou seja, não recarrega a página. Assim, conseguimos manipular os dados sem perder o que já foi digitado.

Depois, o código captura o que foi escrito no campo de nome e guarda esse valor em uma variável chamada `nome`. O mesmo é feito com o campo de email, que é salvo em uma variável chamada `email`.

Em seguida, o código encontra o corpo da tabela com o ID `tabelaCadastro`, focando no elemento `<tbody>`. Com isso, ele insere uma nova linha na tabela.

Duas células são criadas nessa nova linha: uma para o nome do usuário e outra para o email. O conteúdo de cada célula é preenchido com os valores que foram guardados nas variáveis `nome` e `email`.

Por fim, o formulário é resetado, ou seja, todos os campos são limpos, permitindo que o usuário insira novas informações facilmente.
