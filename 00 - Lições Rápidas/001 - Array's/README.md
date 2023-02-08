> - ---
> * 🚧⛔ | ⚠️ | 🚩 | 🏁 | 🏁❗ | ✔️ | ✅ | ▶️ | ✏️ | ✍️ | 📍
> - ---

>
> ### **✏️ 01.00 Array (matriz) em javascript**
> #### **Descrição**
>
>     Uma matriz em JavaScript é uma estrutura de dados que contém uma coleção de
>     valores (elementos) que podem ser de qualquer tipo de dados (número, string,
>     objeto, etc.). Arrays são declarados usando colchetes []e cada elemento é
>     separado por uma vírgula. Por exemplo:
>
> ---
>#### ***✍️ Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3, 4, 5];
> let names = ['John', 'Jane', 'Jim'];
>
> ```
>     Arrays em JavaScript são dinâmicos e podem ser modificados adicionando,
>     removendo ou atualizando elementos. Você pode acessar elementos em um array
>     usando um índice, que começa em 0. Por exemplo:
> ---
>#### ***✍️Exemplo de código JS***
> ``` JS
> console.log(numbers[0]); // 1
> console.log(names[1]); // Jane
>
> ```
>     Arrays JavaScript têm muitos métodos embutidos úteis como push(), pop(),
>     shift(), unshift(), slice(), splice(), sort(), reverse()etc. que podem ser
>     usados ​​para executar várias operações em arrays.
>

> ### **📍 01.01 Exemplo de inserir elementos em um array.**
> #### **Descrição**
>     Aqui está uma explicação detalhada de cada método usado para adicionar
>     elementos a uma matriz em JavaScript:
>  ---
>  1. push()método: Adiciona um elemento ao final de um array. Ele retorna o novo
>     comprimento do array.
>
>
>##### ***✍️Exemplo de código JS***
> ``` JS
>  let numbers = [1, 2, 3];
>  let newLength = numbers.push(4);
>  console.log(numbers); // [1, 2, 3, 4]
>  console.log(newLength); // 4
>
> ```
> ---
> 2. unshift()método: Adiciona um ou mais elementos ao início de um array.
>    Ele retorna o novo comprimento do array.
>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> let newLength = numbers.unshift(0);
> console.log(numbers); // [0, 1, 2, 3]
> console.log(newLength); // 4
>
> ```
>
>
> ---
> 3. splice()método: adiciona elementos a uma matriz em uma posição especificada e também
    pode remover elementos. O primeiro argumento é o índice inicial, o segundo argumento é
    o número de elementos a serem removidos (se houver) e o restante dos argumentos são
    os elementos a serem adicionados. Ele retorna uma matriz dos elementos removidos.
>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> let removed = numbers.splice(1, 0, 1.5);
> console.log(numbers); // [1, 1.5, 2, 3]
> console.log(removed); // []
>
> ```
>
> ---
> 4. Operador de atribuição: atribua diretamente um valor a um índice em uma matriz. Esse método também pode ser usado para adicionar elementos ao final de uma matriz usando um índice maior que o último índice.
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> numbers[3] = 4;
> console.log(numbers); // [1, 2, 3, 4]
>
> ```
>
