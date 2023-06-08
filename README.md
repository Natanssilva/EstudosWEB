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
 
 ## HTML
   - Pra fazer download pelo html, basta usar o atributo "download" na tag <a> mas só irá funcionar se o arquivo estiver no servidor
      -Se atribuir um valor de texto depois do atributo como por exemplo download = "foto google" esse será o nome que irá aparecer no explorer na hora de salvar o arquivo
  - Para ser direcionado ao app para enviar um email deverá usar o dentro da tag <a> a seguinte forma:
  - <a> href = "mailto:name@email.com">qualquer coisa </a> 
      - Lembrando que para automatizar e enviar um email direto no click do usuário precisará de uma linguagem de programação
  -Tambem é possivel colocar um assunto e mensagem no corpo já definidos dentro da tag <a> por exemplo:
    - <a> href = "mailto:name@email.com?subject=Reuniao da proxima semana">qualquer coisa </a>  
      - Esse exemplo colocará como assunto do email
    - <a> href = "mailto:name@email.com?subject=Reuniao da proxima semana&body=Na proxima semana a reuniao será as 14h">qualquer coisa </a> 
      - Esse exemplo manterá o assunto e adicionará uma mensagem pré definidas

  - TABELAS EM HTML:
    - As tabelas em HTML ficam dentro da tag <table>
      - A estrutura base de uma tabela consiste no seguinte código:
         ``` 
        <table>
        <tr> <!--Table row(linha da tabela)-->
            <td>Coluna 1 - Linha 1</td>
            <td>Coluna 2 - Linha 1</td>
            <td>Coluna 3 - Linha 1</td>
        </tr>
        <tr> <!--Table row(linha da tabela)-->
            <td>Coluna 1 - Linha 2</td>
            <td>Coluna 2 - Linha 2</td>
            <td>Coluna 3 - Linha 2</td>
        </tr>
        <tr> <!--Table row(linha da tabela)-->
            <td>Coluna 1 - Linha 3</td>
            <td>Coluna 2 - Linha 3</td>
            <td>Coluna 3 - Linha 3</td>
        </tr>
       </table> 
       ```
    - E ela será mostrada dessa forma: 
  
         <table>
        <tr> <!--Table row(linha da tabela)-->
            <td>Coluna 1 - Linha 1</td>
            <td>Coluna 2 - Linha 1</td>
            <td>Coluna 3 - Linha 1</td>
        </tr>
        <tr> <!--Table row(linha da tabela)-->
            <td>Coluna 1 - Linha 2</td>
            <td>Coluna 2 - Linha 2</td>
            <td>Coluna 3 - Linha 2</td>
        </tr>
        <tr> <!--Table row(linha da tabela)-->
            <td>Coluna 1 - Linha 3</td>
            <td>Coluna 2 - Linha 3</td>
            <td>Coluna 3 - Linha 3</td>
        </tr>
    </table>
  - Possui algumas tags em tabela para maximizar o seu uso e também a utilizacação da linguagem javascript e estilizição com o CSS, como por exemplo a tag <thead> que é o cabeçalho da tabela e <tbody> que é o corpo da tabela
  - Usando essas tags teremos o seguinte código:
    ```
    <table>
        <thead>
            <tr> <!--Table row(linha da tabela)-->
                <th>Coluna 1</th>  <!--table header, tem o mesmo comportamento de um <td> mas define o conteudo como um cabeçalho de uma coluna -->
                <th>Coluna 2</th>
                 <th>Coluna 3</th>
            </tr>
        </thead>
        <tbody>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 1</td>
                <td>Coluna 2 - Linha 1</td>
                <td>Coluna 3 - Linha 1</td>
            </tr>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 2</td>
                <td>Coluna 2 - Linha 2</td>
                <td>Coluna 3 - Linha 2</td>
            </tr>
        </tbody>
    </table>
     ```
  - A tabela será mostrada da seguinte maneira:
      <table>
        <thead>
            <tr> <!--Table row(linha da tabela)-->
                <th>Coluna 1</th>
                <th>Coluna 2</th>
                 <th>Coluna 3</th>
            </tr>
         </thead>
        <tbody>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 1</td>
                <td>Coluna 2 - Linha 1</td>
                <td>Coluna 3 - Linha 1</td>
            </tr>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 2</td>
                <td>Coluna 2 - Linha 2</td>
                <td>Coluna 3 - Linha 2</td>
            </tr>
        </tbody>
     </table>
 - Por ultimo na estrutura base de uma tabela, temos a tag tfoot no qual é o rodapé de uma tabela
    - O código completo ficará dessa maneira:
      ```
       <table>
        <thead>
            <tr> <!--Table row(linha da tabela)-->
                <th>Coluna 1</th>
                <th>Coluna 2</th>
                 <th>Coluna 3</th>
            </tr>
        </thead>
        <tbody>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 1</td>
                <td>Coluna 2 - Linha 1</td>
                <td>Coluna 3 - Linha 1</td>
            </tr>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 2</td>
                <td>Coluna 2 - Linha 2</td>
                <td>Coluna 3 - Linha 2</td>
            </tr>
        </tbody>
        <tfoot> <!-- Rodapé -->
            <tr>
                <td>Rodapé 1</td>
                <td>Rodapé 2</td>
                <td>Rodapé 3</td>
            </tr>
        </tfoot>
    </table>
    ```
  
    - A tabela será mostrada dessa forma:
       <table>
        <thead>
            <tr> <!--Table row(linha da tabela)-->
                <th>Coluna 1</th>
                <th>Coluna 2</th>
                 <th>Coluna 3</th>
            </tr>
        </thead>
        <tbody>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 1</td>
                <td>Coluna 2 - Linha 1</td>
                <td>Coluna 3 - Linha 1</td>
            </tr>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 2</td>
                <td>Coluna 2 - Linha 2</td>
                <td>Coluna 3 - Linha 2</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>Rodapé 1</td>
                <td>Rodapé 2</td>
                <td>Rodapé 3</td>
            </tr>
        </tfoot>
    </table>
  
 - A tag <caption> antes do thead serve para colcoar um titulo na tabela onde ele ja é centralizado de forma automatica. Para estilizar a tabela, além de border no css temos o seletor border-collapse: collapse; que ajuda na estilização
  ```
   <table>
     <caption>TABELA 1</caption>
        <thead>
            <tr> <!--Table row(linha da tabela)-->
                <th>Coluna 1</th>
                <th>Coluna 2</th>
                 <th>Coluna 3</th>
            </tr>
        </thead>
        <tbody>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 1</td>
                <td>Coluna 2 - Linha 1</td>
                <td>Coluna 3 - Linha 1</td>
            </tr>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 2</td>
                <td>Coluna 2 - Linha 2</td>
                <td>Coluna 3 - Linha 2</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>Rodapé 1</td>
                <td>Rodapé 2</td>
                <td>Rodapé 3</td>
            </tr>
        </tfoot>
    </table>
   ```
  
- A tabela será mostrada da seguinte forma:
  
     <table>
        <caption>TABELA 1</caption>
        <thead>
            <tr> <!--Table row(linha da tabela)-->
                <th>Coluna 1</th>
                <th>Coluna 2</th>
                 <th>Coluna 3</th>
            </tr>
        </thead>
        <tbody>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 1</td>
                <td>Coluna 2 - Linha 1</td>
                <td>Coluna 3 - Linha 1</td>
            </tr>
            <tr> <!--Table row(linha da tabela)-->
                <td>Coluna 1 - Linha 2</td>
                <td>Coluna 2 - Linha 2</td>
                <td>Coluna 3 - Linha 2</td>
            </tr>
        </tbody>
        <tfoot>
            <tr>
                <td>Rodapé 1</td>
                <td>Rodapé 2</td>
                <td>Rodapé 3</td>
            </tr>
        </tfoot>
    </table>
- Dentro da tag <td> podemos usar dois atributos, colspan = "x" e rowspan = "x"
    - colspan mostra que o numero dentro das aspas significa que a célula vai ocupar x colunas
    - rowspan na mesma lógica, significa que vai ocupar x linhas
