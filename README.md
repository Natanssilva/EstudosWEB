# EstudosWEB
Repositório com conteúdo sobre CSS, HTML, BOOTSTRAP


## CSS
  - Pseudo-Classes: São classes que definem um estado a um elemento e são sempre acompanhadas de : 1x( 2 pontos), por exemplo a classe "hover":
  - .layout: hover{ color: red;}
    - Alguns exemplos de pseudo-classes: hover, active e visited
      - Hover: é um estado quando passa por cima do elemento
      - Active: muda o elemento quando ele é ativado, por exemplo, a cor do link fica outra quando clica nele
      - Visited: muda o elemento depois de ser visitado, por exemplo, depois q clica em um link, a cor dele muda quando retorna a página
  - Pseudo-Elementos : sao palavres chaves adicionadas ao seletor que permite dar estilo a uma parte especifica de um determinado elemento. Acompanhado de :: (2x 2 pontos)
    - Exemplos de Pseudo-Elementos: first-letter / first-line
      - Imagine que temos um texto em uma tag HTML H1 e quero mudar a cor da primeira letra ou da primeira linha, nesse caso utilizamos os pseudos-elementos para estilizar uma parte epescifica do elemento H1
        -  h1::first-line{color:red; font-size:60px;}
          - Nesse código, só a primeira linha vai seguir as regras atribuidas.
   - No css é possivel sobrepor uma regra com o !important do lado do atributo:
      - Color: red !important;
        -  Isso vai sobrepor qualquer outro color que havia sido declarado antes ou depois, logo com !important ele sobrepoe a a ordem.
