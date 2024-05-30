# Condições

Em Dart, as condições são usadas para tomar decisões no fluxo de execução do programa. Existem várias maneiras de expressar condições em Dart, incluindo instruções `if`, `else`, `else if` e `switch`. Aqui estão os detalhes sobre cada uma delas:

## if
A estrutura `if` é usada para executar um bloco de código se uma condição for verdadeira:

~~~dart
void main() {
  int idade = 15;

  if (idade > 17) {
    print('é maioridade');
  }
}
~~~

## else
O `else` é usado para executar um bloco de código se a condição `if` for falsa:

~~~dart
void main() {
  int idade = 15;

  if (idade > 17) {
    print('é maioridade');
  } else {
    print('ainda não é maioridade');
  }
}
~~~

## else if
O `else if` é usado para testar múltiplas condições:

~~~dart
void main() {
  int idade = 15;

  if (idade > 17) {
    print('é maioridade');
  } else if (idade > 11) {
    print('é adolescente');
  }
}
~~~


## switch
A estrutura `switch` é usada para selecionar uma entre várias opções de execução. É útil quando há muitas condições para comparar:

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

~~~dart

void main() {
  int dia = 3;

  switch (dia) {
    case 1:
      print('Segunda-feira');
      break;
    case 2:
      print('Terça-feira');
      break;
    case 3:
      print('Quarta-feira');
      break;
    case 4:
      print('Quinta-feira');
      break;
    case 5:
      print('Sexta-feira');
      break;
    case 6:
      print('Sábado');
      break;
    case 7:
      print('Domingo');
      break;
    default:
      print('Dia inválido');
  }
}
~~~

---
[Índice](README.md)