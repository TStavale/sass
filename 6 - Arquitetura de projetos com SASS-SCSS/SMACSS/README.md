## SMACSS ##

1 - <b>SMACSS</b> é referência que vamos utilizar para arquitetar nosso SASS; <br>
2 - Neste padrão o CSS é dividido em partes; <br>
3 - <b>Base</b>: regras bássicas de estilo, elementos gerais; <br> 
4 - <b>Layout</b>: Elementos que formam a página, ex: header; <br>
5 - <b>Module</b>: Componentes menores; <br>
6 - <b>State</b> e <b>theme</b>: regras que sobrepõe outras e cores do tema.

## Arquivo principal ##

1 - O arquvivo principal vai <b>apenas realizar importações</b>, não vamos adicionar esstilos a ele, isso irá <b>diminuir os imports</b> no nosso arquivo principal; <br>
2 - Podemos chama-ló de <b>main.css</b> ou <b>app.sass</b>; <br>
3 - As pastas de outros módulos iniciam com números, ex: <b>0-plugins</b>.

## Estrutura de pastas ##

1 - Estas são as pastas que vamos criar e também os significados de cada uma; <br>
2 - <b>0-plugins</b>: Frameworks ou códigos de terceiros; <br>
3 - <b>1-base</b>: Arquivo de estilo base; <br>
4 - <b>2-layouts</b>: Arquivos para elementos que formam o layout da página; <br>
5 - <b>3-modules</b>: Componentes das páginas.

## Estilos de base ##

1 - Podemos estilizar tags como: <b>body, a, p</b>; <br>
2 - <b>Não utilizamos</b> classes nem id; <br>
3 - A ideia é <b>pré-estilizar nosso HTML</b>; <br>
4 - Podemos estilizar elementos em arquivos separados.

## Estilos de layout ##

1 - Aqui <b>podemos adicionar ids e classes</b> as regras; <br>
2 - A ideia é estilizar componentes maiores, como o cabeçalho da página (header), main, seciton, aside , footer; <br>
3 - Novamente podemos <b>separar elementos em arquivos distintos</b>.

## Estilos de module ##

1 - Aqui <b>podemos adicionar ids e classes</b> as regras também; <br>
2 - Vamos colocar nossos <b>componentes menores</b>: cards, botões, algum elemento na sidebar; <br>
3 - Podemos também separar cada um deles em um arquivo.