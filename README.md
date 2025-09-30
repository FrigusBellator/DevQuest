Trajetória de Desenvolvimento:
Conceito Inicial: Começamos com um protótipo de fase única, onde criamos o protagonista "Dev", os inimigos "bugs" e a mecânica central dos blocos de perguntas </>.

Correções e Refinamento: Rapidamente identificamos e corrigimos bugs críticos, como problemas de colisão que causavam mortes injustas e falhas na tela de "Game Over". Isso garantiu que a base do jogo fosse sólida.

Expansão para Múltiplas Fases: A grande evolução foi transformar o jogo em uma jornada de três fases, cada uma dedicada a um pilar do desenvolvimento web:

Fase 1: JavaScript

Fase 2: HTML

Fase 3: CSS
Nesta etapa, expandimos o design dos níveis para incluir um total de 25 blocos de perguntas, tornando a exploração mais rica.

Adição de Mecânicas de Jogo: Para aumentar o desafio e a estratégia, implementamos:

Um sistema de vidas, onde errar perguntas ou tocar em inimigos tinha consequências.

Um sistema de pontuação para recompensar o jogador por derrotar os "bugs".

Personalidade e Recompensas: Demos vida ao jogo com toques de personalidade. O protagonista "Dev" foi redesenhado para se assemelhar ao icônico Sheldon Cooper. Criamos também um sistema de recompensa poderoso: a skin "Sheldon Flash", um prêmio para quem acerta todas as perguntas de uma fase, concedendo uma vida extra e invencibilidade.

// --- Banco de Questões do Jogo ---

const jsQuestions = [
    { question: "Qual o resultado de '2' + 2 em JS?", options: ["4", "22", "Erro", "NaN"], answer: 1 },
    { question: "Como se escreve um comentário de UMA linha?", options: ["// Comentário", "/* Comentário */", "<!-- Comentário -->", "# Comentário"], answer: 0 },
    { question: "Qual função imprime algo no console?", options: ["print()", "log()", "console.log()", "debug()"], answer: 2 },
    { question: "O que o operador `||` representa?", options: ["E lógico", "OU lógico", "Negação", "Igualdade"], answer: 1 },
    { question: "Qual método remove o último elemento de um array?", options: [".pop()", ".shift()", ".push()", ".slice()"], answer: 0 },
    { question: "Qual palavra-chave declara uma variável que não pode ser reatribuída?", options: ["var", "let", "const", "static"], answer: 2 },
    { question: "O que `Math.random()` retorna?", options: ["Um nº entre 0 e 10", "Um nº entre 0 e 1", "Um nº inteiro", "Um nº negativo"], answer: 1 },
    { question: "Como se declara uma variável em JavaScript?", options: ["var, let, const", "variable", "v", "let const"], answer: 0 },
];

const htmlQuestions = [
    { question: "Qual tag é usada para o maior título?", options: ["<h6>", "<p>", "<h1>", "<title>"], answer: 2 },
    { question: "Qual tag cria uma lista NÃO ordenada?", options: ["<ol>", "<li>", "<ul>", "<dl>"], answer: 2 },
    { question: "Qual atributo especifica o destino de um link?", options: ["src", "link", "target", "href"], answer: 3 },
    { question: "Qual tag é usada para inserir uma imagem?", options: ["<image>", "<pic>", "<img>", "<figure>"], answer: 2 },
    { question: "Qual o propósito da tag `<head>`?", options: ["Conteúdo principal", "Cabeçalho da página", "Metadados e links", "Rodapé"], answer: 2 },
    { question: "Como se cria um campo de entrada de texto?", options: ["<input type='text'>", "<textfield>", "<input type='button'>", "<text>"], answer: 0 },
    { question: "Qual tag define uma quebra de linha?", options: ["<break>", "<lb>", "<br>", "<hr>"], answer: 2 },
    { question: "Qual tag é usada para criar um botão?", options: ["<input type='button'>", "<button>", "Ambas estão corretas", "Nenhuma está correta"], answer: 2 },
    { question: "Qual tag define o corpo do documento HTML?", options: ["<body>", "<head>", "<!DOCTYPE html>", "<html>"], answer: 0 },
];

const cssQuestions = [
    { question: "Qual propriedade altera a cor de fundo?", options: ["color", "background-color", "font-color", "bgcolor"], answer: 1 },
    { question: "O que a propriedade `display: none;` faz?", options: ["Aumenta o elemento", "Esconde o elemento", "Deixa transparente", "Muda a fonte"], answer: 1 },
    { question: "O que o código `p { font-weight: bold; }` faz?", options: ["Muda a cor", "Aumenta a fonte", "Deixa em itálico", "Deixa em negrito"], answer: 3 },
    { question: "Qual a diferença entre `margin` e `padding`?", options: ["Não há diferença", "Cor vs. Fundo", "Espaço externo vs. Interno", "Fonte vs. Tamanho"], answer: 2 },
    { question: "Para que serve o seletor `:hover`?", options: ["Selecionar o primeiro item", "Estilo ao passar o mouse", "Estilo ao clicar", "Selecionar o último item"], answer: 1 },
    { question: "O que `position: absolute;` faz?", options: ["Posiciona relativo à tela", "Posiciona relativo ao pai", "Centraliza o elemento", "Remove o elemento"], answer: 1 },
    { question: "Qual a função do `z-index`?", options: ["Define a largura", "Define a altura", "Controla a sobreposição", "Define a rotação"], answer: 2 },
    { question: "O que `flex-direction: column;` faz?", options: ["Itens em linha", "Itens em coluna", "Inverte a ordem", "Justifica o conteúdo"], answer: 1 },
    { question: "Como você seleciona um elemento com id 'titulo'?", options: ["#titulo", ".titulo", "titulo", "*titulo"], answer: 0 },
];
