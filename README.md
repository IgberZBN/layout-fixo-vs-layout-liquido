# Layout fixo Vs layout fluido

## Explicando alguns conceitos antes de usar layout fluido:

>### Primeiramente precisamos entender alguns conceitos do CSS:
>#### Funções:
>- [clamp](#clamp)
>- [max/min](#maxAndMin)
>#### Medidas:
>- [%](#porcentagem)
>- [vw](#vw)
>- [em](#em)



>##### <a id="clamp"></a>Clamp:
>clamp() é uma função de CSS que permite limitar um valor dentro de um intervalo específico. Ele tem a seguinte sintaxe:
>```css
>    clamp(valor,minimo maximo)
>```
>Onde valor é o valor que deseja-se limitar, minimo é o valor mínimo permitido e maximo é o valor máximo permitido. Se valor for menor que minimo, ele será definido como minimo. Se valor for maior que maximo, ele será definido como maximo. Caso contrário, valor será mantido inalterado.
>##### Exemplo:
>```css
> .exemplo {
>   font-size: clamp(2.5rem, 1rem, 2rem);
>}
>```
>Neste exemplo, se o valor de font-size for menor que 1rem, será definido como 1rem. Se o valor for maior que 2rem, será definido como 2rem. Caso contrário, será definido como 2.5rem.



>##### <a id="maxAndMin"></a>Max/Min:
>Em CSS, as propriedades max-* e min-* são usadas para especificar limites máximos e mínimos para tamanhos de elementos.
>
>A propriedade max-width especifica o tamanho máximo da largura de um elemento. Por exemplo, se você definir max-width: 200px, o elemento nunca será maior do que 200 pixels de largura, mesmo que o conteúdo dentro dele seja maior.
>
>Da mesma forma, a propriedade max-height especifica o tamanho máximo da altura de um elemento.
>
>Por outro lado, a propriedade min-width especifica o tamanho mínimo da largura de um elemento. Por exemplo, se você definir min-width: 200px, o elemento nunca será menor do que 200 pixels de largura, mesmo que o conteúdo dentro dele seja menor.
>Da mesma forma, a propriedade min-height especifica o tamanho mínimo da altura de um elemento.
>
>É possível usar essas propriedades juntas para garantir que um elemento tenha um tamanho mínimo e máximo ao mesmo tempo.
>##### Exemplo:
>```css
>div {
>  min-width: 200px;
>  max-width: 400px;
>}
>```
