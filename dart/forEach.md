# forEach

Em Dart, o método `forEach` é utilizado para iterar sobre elementos de uma coleção, como listas, conjuntos ou mapas. Ele permite aplicar uma função a cada elemento da coleção, fornecendo uma maneira concisa e legível de realizar operações em todos os elementos da coleção.

### Uso do `forEach` em Listas

~~~dart

void main() {
  List<String> frutas = ['maçã', 'banana', 'laranja'];

  frutas.forEach((fruta) {
    print(fruta);
  });
}

// maçã
// banana
// laranja
~~~

Neste exemplo, a função anônima `(fruta) { print(fruta); }` é aplicada a cada elemento da lista `frutas`. A saída será:

### Uso do `forEach` em Conjuntos

~~~dart

void main() {
  Set<int> numeros = {1, 2, 3};

  numeros.forEach((numero) {
    print(numero);
  });
}

// 1
// 2
// 3
~~~

### Uso do `forEach` em Mapas

Para mapas (`Map`), o `forEach` itera sobre os pares chave-valor. A função passada para `forEach` recebe dois argumentos: a chave e o valor.

~~~dart

void main() {
  Map<String, int> idade = {
    'Alice': 30,
    'Bob': 25,
    'Charlie': 35
  };

  idade.forEach((nome, anos) {
    print('$nome tem $anos anos.');
  });
}

// Alice tem 30 anos.
// Bob tem 25 anos.
// Charlie tem 35 anos.
~~~

### Resumo

O método `forEach` é uma maneira conveniente de iterar sobre coleções em Dart, aplicando uma função a cada elemento. Ele é ideal para iterações simples onde não é necessário alterar o fluxo de controle (como usar `break` ou `continue`). Para casos onde mais controle é necessário, o loop `for-in` pode ser mais adequado.

---

[Índex](../README.md)