# Variáveis

## Tipos de Variáveis

Dart é uma linguagem de programação fortemente tipada, o que significa que cada variável tem um tipo associado que determina os valores que a variável pode armazenar e as operações que podem ser realizadas nela. Aqui estão os principais tipos de variáveis em Dart:

### Tipos Numéricos

#### int
Representa números inteiros. Pode armazenar valores positivos e negativos, incluindo zero.

~~~dart

int idade = 30;
~~~

#### double
Representa números de ponto flutuante (decimais).

~~~dart

double valor = 29.99;
~~~

### Tipo Strings

#### String
Representa uma sequência de caracteres. Strings podem ser definidas usando aspas simples ou duplas.

~~~dart

String nome = "Alice";
String texto = 'Olá mundo!';
~~~

### Tipo Booleano

#### bool
Representa valores booleanos. Pode ser verdadeiro (`true`) ou falso (`false`).

~~~dart

bool casado = true;
~~~

### Tipos de Coleção

#### List
Representa uma lista ordenada de elementos. Pode ser uma lista homogênea (todos os elementos do mesmo tipo) ou heterogênea.

~~~dart

List<int> numeros = [1, 2, 3, 4, 5];
~~~

#### Set
Representa uma coleção de elementos únicos. *Não garante a ordem dos elementos.*

~~~dart

Set<String> frutas = {'maçã', 'banana', 'laranja','uva'};
~~~

#### Map
Representa uma coleção de pares chave-valor.

~~~dart

Map<String, int> pontos = {'Alice': 90, 'Bob': 85, 'José': 43};
~~~

### Tipo dinâmico

#### dynamic
Representa uma variável cujo tipo é determinado em tempo de execução. Pode armazenar qualquer tipo de valor, mas seu uso deve ser feito com cuidado.

~~~dart

dynamic teste = 'texto';
teste = 123;
~~~

#### var
Inferido pelo compilador no momento da atribuição inicial. Após a atribuição, o tipo da variável não pode ser alterado.

~~~dart

var idade = 30;
var nome = "Alice";
~~~

### Tipo num (Supertipo de int e double)

#### num
É um supertipo de **int** e **double**, usado quando uma variável pode conter tanto um inteiro quanto um número decimal.

~~~dart

num teste = 5;
teste = 5.5;
~~~

---

[Índex](../README.md)