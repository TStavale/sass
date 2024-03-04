## if e else no SASS ##

1 - Podemos criar uma <b>estrutura de condições</b> também no SaSS; <br>
2 - Utilizando o <b>@if</b> criamos a condição e com <b>@else</b> quando a condição do if for falsa; <br>
3 - Temos também a opção de <b>@else if</b>; <br>
4 - Estass regras funcionam como em outras linguagens de programação; <br>
5 - Ex:

    @function calc-func($a, $b)

        $result: 0
        
        @if $a > $b 
            $result: red
        @else if $a < $b 
            $result: blue
        @else
            $result: green

        @return $result

## each no SASS ##

1 - Podemos criar uma <b>estrutura de repetição em listas</b> no SASS também; <br>
2 - Utilizando <b>@each</b> criamos a estrutura; <br>
3 - Podemos repetir uma <b>criação de classe n vezes</b>, por exmplo:

    $fonts: 40px, 60px, 100px

    @each $font in $fonts
        .title-#{$font}
            font-size: $font
            line-height: $font * 1.2

4 - Veja a sintaxe (onde <b>$sizes</b> é a lista de valores):

    @each $size in $sizes


## for no SASS ##

1 - Aqui criaremos uma <b>estrutura de repetição</b> utilizando <b>@for</b> podemos repeti-lá quantas vezes for necessária, por meio de uma condição; <br>
2 - Veja a sintaxe:

    @for $i from 1 through 3 (repetir de 1 até chegar a 3)
        código...

3 - Ex:

    @for $i from 1 through 3
        .p-#{$i}
            @if $i == 1
                color: lightblue
            @else if $i == 2
                color: lightgreen
            @else if $i == 3
                color: teal
            background-color: #000
    

sass --watch sass/styles.sass:css/styles.css