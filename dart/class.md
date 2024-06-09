# Classes & Objetos

## Classe

Classe é uma estrutura fundamental usada para criar objetos. As classes definem um tipo de dado, encapsulando dados (atributos) e comportamento (métodos) que os objetos desse tipo terão. Isso permite a criação de instâncias de objetos que possuem propriedades e comportamentos específicos definidos pela classe.

### Definição de uma Classe
Aqui está um exemplo básico de como definir uma classe em Dart:

~~~dart

// Classe Humano
class Humano {  
  // Atributos  
  String nome;  
  int idade;

  // Construtor  
  Humano(this.nome, this.idade);

  // Métodos  
  void apresentar() {  
    print('Olá, meu nome é $nome e eu tenho $idade anos.');  
  }  
}

void main() {  
  // Criando uma instância da classe Humano  
  Humano pessoa1 = Humano('João', 30);  
  pessoa1.apresentar(); // Olá, meu nome é João e eu tenho 30 anos.  
}
~~~

~~~dart

class Song {
  String name;
  String autor;
  String key;
  
  Song(this.name, this.autor, this.key);
}

void main() {
  Song music01 = Song('Minha Música','Samuel Santana','C#m');
  print('${music01.name} - ${music01.key}'); // Minha Música - C#m
}
~~~

---

[Índex](../README.md)