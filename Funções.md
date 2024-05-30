# Funções

Em Dart, uma função é um bloco de código reutilizável que pode ser chamado com um nome. As funções podem aceitar parâmetros e retornar um valor.

### Funções sem retorno
As funções que não precisam retornar algum valor, inicia com a palavra-chave `void`.

~~~dart

void main() {
  saudacao();
}

void saudacao() {
  print('Olá, mundo!');
}
~~~

~~~dart
void main() {
  saudacao();
}

void saudacao() => print('Olá, mundo!');
~~~

### Funções com Parâmetros
As funções podem aceitar parâmetros para receber valores na hora da chamada.

~~~dart

void main() {
  saudacao('João');
  saudacao('Maria');
}

void saudacao(String nome) {
  print('Olá, $nome!');
}
~~~

## Funções com Retorno
As funções podem retornar um valor usando a palavra-chave `return`. O tipo de retorno é declarado antes do nome da função.

~~~dart

void main() {
  int resultado = soma(5, 3);
  print('A soma é: $resultado');
}

int soma(int a, int b) {
  return a + b;
}
~~~

~~~dart

int soma(int a, int b) => a + b;
~~~

~~~dart

void main() {
  print(saudacao('José'));
}

String saudacao(String nome) {
  String frase = 'Olá $nome';
  return frase;
}
~~~


## Mais  exemplos de funções

~~~dart

void main() {
  idade('José',1997); // Olá José, voce tem 27 anos de idade.
}

void idade(String name, int ano) {
  int anoAtual = 2024;
  print('Olá $name, voce tem ${anoAtual - ano} anos de idade.');
}
~~~

---

[Índice](README.md)
