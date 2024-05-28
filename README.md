# Minha Documentação

Dart é uma linguagem de programação fortemente tipada, o que significa que cada variável tem um tipo associado que determina os valores que a variável pode armazenar e as operações que podem ser realizadas nela. Aqui estão os principais tipos de variáveis em Dart:

## Variáveis

### Tipos Numéricos

**int:** Representa números inteiros. Pode armazenar valores positivos e negativos, incluindo zero.

~~~dart

int idade = 30;
~~~

**double:** Representa números de ponto flutuante (decimais).

~~~dart

double preco = 29.99;
~~~

### Tipo Strings

**String:** Representa uma sequência de caracteres. Strings podem ser definidas usando aspas simples ou duplas.

~~~dart

String nome = "Alice";
String text = 'Hello, World!';
~~~

### Tipo Booleano

**bool:** Representa valores booleanos. Pode ser verdadeiro (`true`) ou falso (`false`).

~~~dart

bool aprovado = true;
~~~

### Tipos de Coleção

**List:** Representa uma lista ordenada de elementos. Pode ser uma lista homogênea (todos os elementos do mesmo tipo) ou heterogênea.

~~~dart

List<int> numeros = [1, 2, 3, 4, 5];
~~~

**Set:** Representa uma coleção de elementos únicos. Não garante a ordem dos elementos. 

~~~dart

Set<String> frutas = {'maçã', 'banana', 'laranja'};
~~~

**Map:** Representa uma coleção de pares chave-valor.

~~~dart

Map<String, int> pontos = {'Alice': 90, 'Bob': 85};
~~~

### Tipo dinâmico

**dynamic:** Representa uma variável cujo tipo é determinado em tempo de execução. Pode armazenar qualquer tipo de valor, mas seu uso deve ser feito com cuidado.

~~~dart

dynamic teste = 'texto';
teste = 123;
~~~

**var:** Inferido pelo compilador no momento da atribuição inicial. Após a atribuição, o tipo da variável não pode ser alterado.

~~~dart

var idade = 30;
var nome = "Alice";
~~~

### Tipo num (Supertipo de int e double)

**num:** É um supertipo de **int** e **double**, usado quando uma variável pode conter tanto um inteiro quanto um número de ponto flutuante.

~~~dart

num test = 5;
teste = 5.5;
~~~

## Switch

~~~dart

void main() {
  bool resultado = true;

  switch (resultado) {
    case true:
      print('Aprovado');
      break;
    case false:
      print('Reprovado');
      break;
  }
}
~~~

~~~
Aprovado

Process finished.
~~~

## Loops

~~~dart

for (var i = 0; i < 5; i++){
  print('Dart');
}
~~~

~~~dart

var i = 0;
while (i < 5){
  print('Dart');
  i++;
}
~~~

## Funções

~~~dart

void main(){
  print(somar(3,2));
}

int somar(int x, int y){
  return x + y;
}
~~~

~~~
5

Process finished.
~~~

~~~dart

void main(){
  print(bloco('@'));
  print(bloco('#'));
  print(bloco('&'));
}

String bloco(String a){
  String b = '';
  for (int i = 0; i < 10; i++){
    b = b + a;
  }
  
  return b + '\n';
}
~~~

~~~
@@@@@@@@@@

##########

&&&&&&&&&&


Process finished.
~~~

~~~dart

void main(){
  String bloco = "@";
  desenhar(bloco);
}

void desenhar (bloco){
  String a = "          ";
  String b = "";

  for ( int i = 0; i <= 9; i++){
    a = a.substring(0, a.length - 1 );
    b = b + bloco + " ";
    print( a + b );
  }
}
~~~

~~~
         @ 
        @ @ 
       @ @ @ 
      @ @ @ @ 
     @ @ @ @ @ 
    @ @ @ @ @ @ 
   @ @ @ @ @ @ @ 
  @ @ @ @ @ @ @ @ 
 @ @ @ @ @ @ @ @ @ 
@ @ @ @ @ @ @ @ @ @ 

Process finished.
~~~
