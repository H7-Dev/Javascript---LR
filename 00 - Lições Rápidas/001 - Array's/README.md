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
>##### ***✍️Exemplo de código JS***
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
>###### ***✍️Exemplo de código JS***
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
>###### ***✍️Exemplo de código JS***
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
>###### ***✍️Exemplo de código JS***
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
>###### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> numbers[3] = 4;
> console.log(numbers); // [1, 2, 3, 4]
>
> ```

> ### **📍 01.02 Exemplo de modificar elementos em uma matriz em JavaScript:**
>
> ---
> 1. Usando o operador de atribuição: atribua diretamente um valor a um índice na matriz.
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> numbers[1] = 1.5;
> console.log(numbers); // [1, 1.5, 3]
>
> ```
> ---
>  2. Usando o splice()método: Modifica elementos em uma matriz em uma posição especificada e também pode adicionar ou remover elementos. O primeiro argumento é o índice inicial, o segundo argumento é o número de elementos a serem removidos (se houver) e o restante dos argumentos são os elementos a serem adicionados. Ele retorna uma matriz dos elementos removidos.
>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> let removed = numbers.splice(1, 1, 1.5);
> console.log(numbers); // [1, 1.5, 3]
> console.log(removed); // [2]
>
> ```
>
> ---
> 3. Usando o map()método: Cria um novo array aplicando uma função a cada elemento do array original.
>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> let doubledNumbers = numbers.map(function(number) {
>   return number * 2;
> });
> console.log(doubledNumbers); // [2, 4, 6]
> ```
>
> 4. Usando um loop: modifique os elementos em uma matriz usando um loop como forou forEach.
>
> ---
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> for (let i = 0; i < numbers.length; i++) {
>   numbers[i] = numbers[i] * 2;
> }
> console.log(numbers); // [2, 4, 6]
>
> ```


> ### **📍 01.03 Exemplo de como remover elementos de um array**
>
> 1. Usando o pop()método: Remove o último elemento de um array e retorna o elemento removido.
>
>##### ***✍️Exemplo de código JS***
>``` JS
> let numbers = [1, 2, 3];
> let last = numbers.pop();
> console.log(numbers); // [1, 2]
> console.log(last); // 3
>
> ```
> ---
> 2. Usando o shift()método: Remove o primeiro elemento de um array e retorna o elemento removido.
>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> let first = numbers.shift();
> console.log(numbers); // [2, 3]
> console.log(first); // 1
>
> ```
> ---
>
> 3. Usando o splice()método: Remove elementos de uma matriz em uma posição especificada e também pode adicionar ou modificar elementos. O primeiro argumento é o índice inicial, o segundo argumento é o número de elementos a serem removidos e o restante dos argumentos são os elementos a serem adicionados. Ele retorna uma matriz dos elementos removidos.
>
>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3];
> let removed = numbers.splice(1, 1);
> console.log(numbers); // [1, 3]
> console.log(removed); // [2]
>
>```
>
> ---
> 4.   Usando o filter()método: Cria uma nova matriz que inclui apenas elementos que passam em um determinado teste.
>
>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [1, 2, 3, 4, 5];
> let evenNumbers = numbers.filter(function(number) {
>   return number % 2 === 0;
> });
> console.log(evenNumbers); // [2, 4]
>
> ```
>     Nesse último trecho de código é um exemplo de como remover elementos de um array usando o filter()método. O filter()método cria uma nova matriz que inclui apenas elementos que passam em um determinado teste, especificado pela função fornecida.
>     Neste exemplo, a função verifica se cada elemento da numbersmatriz é divisível por 2 usando o módulo operador %. Se o resultado for 0, significa que o número é par e será incluído no novo array evenNumbers. O filter()método retorna uma nova matriz que contém apenas números pares da numbersmatriz original.
>     Portanto, esse trecho de código filtra todos os números ímpares da numbersmatriz e armazena apenas os números pares na evenNumbersmatriz.
>
> ---


> ### **📍 01.04 Exemplo de como o sort ()  de um array**
> #### **Descrição**
>
>    O sort()método é uma função interna em JavaScript que classifica os elementos de uma matriz
>    no local e retorna a matriz classificada. Por padrão, o sort()método classifica os
>    elementos de uma matriz como strings, o que pode causar resultados inesperados para números.
>
>    Exemplo:
>>
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [3, 1, 2];
> numbers.sort();
> console.log(numbers); // [1, 2, 3]
>
> ```
>   * Se você deseja classificar os elementos de uma matriz de números, precisa fornecer uma função de comparação como argumento para o sort()método. Esta função de comparação deve retornar um valor menor que 0 se o primeiro argumento deve ser classificado antes do segundo argumento, 0 se os dois argumentos forem iguais ou um valor maior que 0 se o primeiro argumento deve ser classificado após o segundo argumento.
>##### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [3, 1, 2];
> numbers.sort(function(a, b) {
>   return a - b;
> });
> console.log(numbers); // [1, 2, 3]
>
> ```
>
>     Aqui estão alguns exemplos de como usar o sort()método preservando o array original:
>
> 1. Usando o slice()método:
>
>##### ***✍️Exemplo de código JS***
>``` JS
> let numbers = [3, 1, 2];
> let sortedNumbers = numbers.slice().sort(function(a, b) {
>   return a - b;
> });
> console.log(numbers); // [3, 1, 2]
> console.log(sortedNumbers); // [1, 2, 3]
> ```
>     Neste exemplo, sortedNumbersé uma nova matriz criada cortando a numbersmatriz original e, em seguida, classificando-a usando o sort()método. Desta forma, a numbersmatriz original permanece inalterada.
>
> 2. Usando o operador de propagação ( ...):
> ---
>#### ***✍️Exemplo de código JS***
> ``` JS
> let numbers = [3, 1, 2];
> let sortedNumbers = [...numbers].sort(function(a, b) {
>   return a - b;
> });
> console.log(numbers); // [3, 1, 2]
> console.log(sortedNumbers); // [1, 2, 3]
>
> ```
>
> Neste exemplo, sortedNumbersé uma nova matriz criada espalhando os elementos da numbersmatriz original em uma nova matriz e, em seguida, classificando-a usando o sort()método. Desta forma, a numbersmatriz original permanece inalterada.
