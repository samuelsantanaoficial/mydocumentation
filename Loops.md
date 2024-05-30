# Loops


## for
O loop `for` é usado quando você sabe de antemão quantas vezes deseja executar um bloco de código. A estrutura do loop `for` inclui uma inicialização, uma condição e um incremento/decremento.

~~~dart

void main() {
  for (int i = 0; i < 5; i++) {
    print('Contagem: $i');
  }
}
~~~

## for-in
O loop `for-in` é usado para iterar sobre os elementos de uma coleção (por exemplo, uma lista ou um conjunto).

~~~dart

void main() {  
  var dias = [1, 2, 3, 4, 5, 6, 7];  
  for (int x in dias) {  
    print('Dia: $x');  
  }  
}
~~~

~~~dart

void main() {
  List<String> dias = ['domingo','segunda','terça','quarta','quinta','sexta','sábado'];
  for (String x in dias) {
    print('Dia: $x');
  }
}
~~~


## while
O loop `while` executa um bloco de código enquanto uma condição específica for verdadeira. A condição é avaliada antes de cada iteração do loop.

~~~dart

void main() {
  int contador = 0;
  
  while (contador < 5) {
    print('Contagem: $contador');
    contador++;
  }
}
~~~


## do-while
O loop `do-while` é semelhante ao loop `while`, mas a condição é avaliada após a execução do bloco de código, garantindo que o bloco de código seja executado pelo menos uma vez.

~~~dart

void main() {
  int contador = 0;
  
  do {
    print('Contagem: $contador');
    contador++;
  } while (contador < 5);
}
~~~

## Loops com break e continue

### break
A instrução `break` é usada para sair imediatamente de um loop, ignorando qualquer iteração restante.

~~~dart

void main() {
  for (int i = 0; i < 10; i++) {
    print('Contagem: $i');
    if (i == 5) {
      break;
    }
  }
}
~~~

### continue
A instrução `continue` é usada para pular a iteração atual e passar para a próxima iteração do loop.

~~~dart

void main() {
  List<int> numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

  for (int x in numeros) {
    // Se o número for par,
    // pular esta iteração do loop
    if (x % 2 == 0) {
      continue;
    }
    // Caso contrário,
    // imprimir o número ímpar
    print('Número ímpar: $x');
  }
}
~~~

---

[Índice](README.md)