## Mixins ##

1 - São como funções, podemos definir um código que poderá ser reutilizado ao longo do projeto; <br>
2 - A sintaxe é: <b>@mixin nome</b> e a baixo aninhado, as regras que desejar; <br>
Podemos criar o mixin no mesmo arquivo do sass ou criar um arquivo apenas para eles e importar ele no projeto principal, ou seja, no arquivo styles.sass.

## Mixins com argumentos ##

1 - Os mixins podem receber <b>argumentos</b>, deixando nosso código ainda mais dinâmico; <br>
2 - Os argumentos devem ficar <b>depois do nome e entre parênteses</b>; <br>
3 - Sintaxe:
    
    @mixin calc($a, $b)

## Argumentos opcionais ##

1 - Os mixins podem receber <b>argumentos opcionais</b>, ou seja, que já tem um valor pré-definido; <br>
2 - Se não passamos um valor, ele vai utilizar o já definido; <br>
3 - Veja: 

    @mixin optional($a, $b: 10)

## Argumentos pelo nome ##

1 - Podemos utilizar um mixin e passar os <b>argumentos pelo seu nome</b>; <br>
2 - Esta técinica é útil <b>quando há vários argumentos opcionais</b>; <br>
3 - Utilizamos desta forma: 

    @include calc(100px, $color: red)

## Herança ##

1 - Podemos criar umaherança com <b>@extend</b>; <br>
2 - É interessante utilizar em conjunto dos <b>placeholder selectors (%)</b>; <br>
3 - Veja um exemplo: 

    %red-button
        regras

    .button
        @extend %red-button

## Operações complexas ##

1 - Podemos realizar <b>operaçõe matemáticas complexas</b> em uma regra de SASS; <br>
2 - O resultado final será calculado e <b>transsferido para CSS</b>; <br>
3 - Veja um exemplo:

    width: 300px / 10px + 5%

    width: 300px / 10px * 2

    width: 300px + (10px / 2)

4 - Pode-se usar variáveis tmabém:

    $medida: 15
    width: 300px * $medida / 3

5 - Só fique atento a qual unidade vocês esta usando, porque não pode misturar as unidades de medidas. E: px, rem em, etc.

sass --watch sass/styles.sass:css/styles.css