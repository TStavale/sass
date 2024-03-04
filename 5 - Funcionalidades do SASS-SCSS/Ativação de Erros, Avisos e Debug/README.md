## Ativação de erros ##

1 - Podemos <b>gerar um erro com o SASS</b>; <br>
2 - Uma situação interessante é, quando criamos uma função e ela precisa de alguns valores mínimos para um argumento; <br>
3 - Então caso o programador não insira corretamente, disparamos um erro com <b>@erro</b>, ex:

    @if $variation > 3
        @error "Insira variações até o número 3"

4 - Podemos <b>interpolar valores</b> na mesma mensagem também.

## Ativação de Avisos (Warning) ##

1 - Podemos <b>gerar um aviso com o SASS</b>; <br>
2 - A situação pode ser a mesma que a do error, mas este método é menos invasivo, ele não para a aplicação, <b>mostra apenas no console</b>; <br>
3 - Então caso o programador não insira corretamente, disparamos um erro com <b>@warn</b>, ex

    $var: 3

    @if $variation > $var
        @warn "O número máximo de variações é #{$var}"

4 - Podemos <b>interpolar valores</b> na mensagem também.

## Ativação de Debug ##

1 - Podemos <b>ativar um bugger no SASS</b>; <br>
2 - A chamada do recurso é por <b>@debug</b>, ex:

    @function custom-width($width: 200px, $division: 2)

        @debug "O valor da divisão é: #{$width / $division}"
    
        @return $width / $division

3 - Vamos imprimir uma mensagem no console, com <b>valores interpolados</b> ou não; <br>
4 - Parecido com o warning, mas serve para <b>depuração de código</b>.