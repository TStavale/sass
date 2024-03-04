## Pré-processador ##

1 - É um software que recebe uma entrada de dados e gera uma saída, normalmente alterando os dados para uma forma que seja aceita por outro software;<br>
2 - O SASS é um pré-processsador de CSS - ele recebe funcionalidades que não são reconhecidas pelo css e transforma em css puro.

## SASS ##

1 - Sendo um pré processador de CSS, ele ajuda a aumentar a produtividade de código para o desenvolvimento web;<br>
2 - Nele poderemos encontrar, variáveiss, mixins, nesting, herança e muito mais;<br>
3 - Com ele poderemos esscrever menos códigos que deixará um css com mais qualidadde;<br>
4 - Projetos grandes utilizam o SASS, como o Bootstrap.

<h4>Benefícios/recursos do SASS</h4>

<ul>
    <li>Geração de CSS otimizado e válido</li>
    <li>Variáveis - que permite o reaproveitamento de estilos e facilidade de manutenção</li>
    <li>Nesting - encadeamento de seletoress de CSS</li>
    <li>Partials - Divisão de responsabilidades no CSS</li>
    <li>Mixins - espécie de função, para reaproveitamento de estilo.</li>
</ul>

## SASS x SCSS x CSS ##

1 - O SASS e o SCSS são bem parecidos, ambos tem o objetivo de trazer novas funcionalidades ao CSS, entretanto o SASS possui mais recursos e tem uma sintaxe mais simples;<br>
2 - É possivel préprocessar SCSS com SASS, no fim todo código gerado vira CSS puro.

## Extensão SASS ##


1 - Nome da extensão é SASS;<br>
2 - Funcionalidades como, auto-complete, highlight de código, formatação e mais.

## Observações sobre o SASS ##

1 - Criar uma pasta sass e um arquivo com a extensão .sass, além da pasta e arquivo de extensão css.<br>
2 - Não é preciso colocar as chaves após o elemento {};<br>
3 - Toda vez que você criar ou modificar algo no arquivo sass, para ele "grudar" no css, você precisa fazer o comando "sass <input.sass> [output.css]" no TERMINAL da pasta RAIZ do projeto. Onde input é o caminho para o arquivo do sass e output é o caminho para o arquivo css. Ex: sass sass/styles.sass css/styles.css. Pasta > Arquivo.<br>
4 - Caso queira, você pode deixar essa atualização do sass com o css automatica, usanso o comando --watch sass/input.sass:css/output.css no mesmo terminal que usou o outro. Ex: sass --watch sass/styles.sass:css/styles.css

## Debug de SASS ##

1 - O debug irá avisar atraves de uma mensagem no terminal ou no proprio navegador que tem um erro em derteminado lugar no código. Basta corrigir o erro e ele volta a funcionar.