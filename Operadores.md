# Operadores Básicos

## Operadores Aritméticos

Os operadores aritméticos são usados para realizar operações matemáticas simples.

- **Adição** (`+`): Soma dois valores.
- **Subtração** (`-`): Subtrai um valor do outro.
- **Multiplicação** (`*`): Multiplica dois valores.
- **Divisão** (`/`): Divide um valor pelo outro e retorna um número de ponto flutuante.
- **Divisão Inteira** (`~/`): Divide um valor pelo outro e retorna um inteiro.
- **Resto** (`%`): Retorna o resto da divisão de dois valores.

~~~dart

void main() {
  int a = 10;
  int b = 4;

  print(a + b);   // 14
  print(a - b);   // 6
  print(a * b);   // 40
  print(a / b);   // 2.5
  print(a ~/ b);  // 2
  print(a % b);   // 2
}
~~~

## Operadores de Incremento e Decremento
Esses operadores são usados para aumentar ou diminuir o valor de uma variável.

- **Incremento** (`++`): Incrementa o valor em 1.
- **Decremento** (`--`): Decrementa o valor em 1.

~~~dart

void main() {
  int a = 5;

  a++;
  print(a);  // 6

  a--;
  print(a);  // 5
}

~~~

## Operadores de Atribuição
Os operadores de atribuição são usados para atribuir valores às variáveis.

- **Atribuição Simples (`=`)**: Atribui um valor à variável.

~~~dart

void main() {
  int pontos = 0;  // 0
  pontos = 5;      // 5
}
~~~

- **Atribuição com Adição (`+=`)**: Soma um valor à variável e atribui o resultado à variável.

~~~dart

void main() {
  int a = 10;

  a += 5;    // a = a + 5
  print(a);  // 15
}
~~~

~~~dart

void main() {
  String a = 'Olá ';

  a += 'mundo!'; // a = a + 'mundo!'
  print(a);      // 'Olá mundo!'
}
~~~

- **Atribuição com Subtração (`-=`)**: Subtrai um valor da variável e atribui o resultado à variável.

~~~dart

void main() {
  int a = 10;
  
  a -= 3;    // a = a - 3
  print(a);  // 7
}
~~~

- **Atribuição com Multiplicação (`*=`)**: Multiplica a variável por um valor e atribui o resultado à variável.

~~~dart

void main() {
  int a = 10;
  
  a *= 2;    // a = a * 2
  print(a);  // 20
}
~~~


- **Atribuição com Divisão (`/=`)**: Divide a variável por um valor e atribui o resultado à variável.

~~~dart

void main() {
  double a = 10;
  
  a /= 6;    // a = a / 6
  print(a);  // 1.6666666
}
~~~

- **Atribuição com Divisão Inteira (`~/=`)**: Divide a variável por um valor e atribui o resultado inteiro à variável.

~~~dart

void main() {
  int a = 10;
  
  a ~/= 3;   // a = a / 3
  print(a);  // 3
}
~~~


- **Atribuição com Resto (`%=`)**: Calcula o resto da divisão da variável por um valor e atribui o resultado à variável.

~~~dart

void main() {  
  int a = 10;  
   
  a %= 3;    // a = resto de 10 / 3
  print(a);  // 1  
}
~~~


## Operadores de Comparação
Os operadores de comparação são usados para comparar dois valores e retornar um booleano (`true` ou `false`).

- **Igualdade (`==`)**: Retorna verdadeiro se os valores forem iguais.
- **Desigualdade (`!=`)**: Retorna verdadeiro se os valores forem diferentes.
- **Maior que (`>`)**: Retorna verdadeiro se o valor da esquerda for maior que o valor da direita.
- **Menor que (`<`)**: Retorna verdadeiro se o valor da esquerda for menor que o valor da direita.
- **Maior ou igual a (`>=`)**: Retorna verdadeiro se o valor da esquerda for maior ou igual ao valor da direita.
- **Menor ou igual a (`<=`)**: Retorna verdadeiro se o valor da esquerda for menor ou igual ao valor da direita.

~~~dart

void main() {
  int a = 10;
  int b = 5;

  print(a == b);  // false
  print(a != b);  // true
  print(a > b);   // true
  print(a < b);   // false
  print(a >= b);  // true
  print(a <= b);  // false
}
~~~

## Operadores Lógicos
Os operadores lógicos são usados para combinar expressões booleanas.

- **E - lógico (`&&`)**: Retorna verdadeiro se ambas as expressões forem verdadeiras.
- **OU - lógico (`||`)**: Retorna verdadeiro se pelo menos uma das expressões for verdadeira.
- **NÃO - lógico (`!`)**: Inverte o valor lógico de uma expressão.

~~~dart

void main() {
  bool x = true;
  bool y = false;

  print(x && y);  // false
  print(x || y);  // true
}
~~~

~~~dart

void main() {
  bool teste = false;
  print(!teste);  // true
}
~~~

---
[Índice](README.md)