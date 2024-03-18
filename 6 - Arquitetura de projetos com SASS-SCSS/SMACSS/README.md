## SMACSS ##

1 - <b>SMACSS</b> é referência que vamos utilizar para arquitetar nosso SASS; <br>
2 - Neste padrão o CSS é dividido em partes; <br>
3 - <b>Base</b>: regras bássicas de estilo, elementos gerais; <br> 
4 - <b>Layout</b>: Elementos que formam a página, ex: header; <br>
5 - <b>Module</b>: Componentes menores; <br>
6 - <b>State</b> e <b>theme</b>: regras que sobrepõe outras e cores do tema.

## Arquivo principal ##

1 - O arquvivo principal vai <b>apenas realizar importações</b>, não vamos adicionar esstilos a ele; <br>
2 - Podemos chama-ló de <b>main.css</b> ou <b>app.sass</b>; <br>
3 - As pastas de outros módulos iniciam com números, ex: <b>0-plugins</b>.


sass --watch sass/main.sass:css/main.css