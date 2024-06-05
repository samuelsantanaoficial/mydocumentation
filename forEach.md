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

---
[Índice](README.md)