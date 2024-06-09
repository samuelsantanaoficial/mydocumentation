# Strings

Uma string pode ser simples ou multilinha. Strings de linha única são escritas usando aspas simples ou duplas correspondentes.

~~~dart

'Aspas simples';
"Aspas dupla";

"É possível usar 'aspas simples' dentro de uma string com aspas dupla";
~~~

Strings de múltiplas linhas são escritas usando aspas triplas. 

~~~dart

'''Uma Strings com
três aspas
Suporta múltiplas linhas''';

"""Uma Strings com
três aspas
Suporta múltiplas linhas""";
~~~

Você pode usar operador (`+`) para concatenar strings:

~~~dart

String str = 'Dart ' + 'é ' + 'legal!';
print(str); // 'Dart é legal!'
~~~

Literais de string adjacentes são concatenados automaticamente:

~~~dart

String str = 'Dart ' 'é ' 'legal!';
print(str); // 'Dart é legal!'
~~~

Você pode usar `${}` para interpolar o valor das expressões Dart em strings. As chaves podem ser omitidas ao usar variáveis:

~~~dart

String str = 'Dart';
print('$str tem ${str.length} letras'); // dart tem 8 letras
~~~

~~~dart

void main() {
  String name = 'Samuel';
  print(name[1]);  //  a
  print(name[2]);  //  m
}
~~~

## Métodos Básicos

### length
Retorna o número de caracteres na string.

~~~dart

String str = "Hello";
print(str.length);  // 5
~~~


### isEmpty
Retorna verdadeiro se a String está vazia.

~~~dart

String str1 = "";
String str2 = "Hello";
print(str1.isEmpty);    // true
print(str2.isEmpty);    // false
~~~

### isNotEmpty
Retorna verdadeiro se a não String está vazia.

~~~dart

String str1 = "";
String str2 = "Hello";
print(str1.isNotEmpty);  // false
print(str2.isNotEmpty);  // true
~~~

## Métodos de Manipulação

### toUpperCase
Converte todos os caracteres da string para maiúsculas.

~~~dart

String str = "Hello";
print(str.toUpperCase()); // "HELLO"
~~~

### toLowerCase
Converte todos os caracteres da string para minúsculas.

~~~dart

String str = "Hello";
print(str.toLowerCase()); // "hello"
~~~

### trim
Remove espaços em branco no início e no final da string.

~~~dart
String str = "  Hello  ";
print(str.trim()); // "Hello"
~~~

### trimLeft
Remove espaços em branco no início da string.

~~~dart
String str = "  Hello  ";
print(str.trimLeft()); // "Hello  "
~~~

### trimRight
Remove espaços em branco no final da string.

~~~dart
String str = "  Hello  ";
print(str.trimRight()); // "  Hello"
~~~

## Métodos de Busca

### contains
Verifica se uma substring está presente na string.

~~~dart

String str = "Hello";
print(str.contains("ell")); // true
~~~


### startsWith

Verifica se a string começa com uma determinada substring.

~~~dart

String str = "Hello";
print(str.startsWith("He")); // true
print(str.startsWith("lo")); // false
~~~


### endsWith

Verifica se a string termina com uma determinada substring.

~~~dart

String str = "Hello";
print(str.endsWith("He")); // false
print(str.endsWith("lo")); // true
~~~

### indexOf
Retorna o índice da primeira ocorrência de uma substring.

~~~dart

String str = "Hello World";
print(str.indexOf("o")); // 4
~~~

### lastIndexOf
Retorna o índice da última ocorrência de uma substring.

~~~dart

String str = "Hello World";
print(str.lastIndexOf("o")); // 7
~~~

## Métodos de Substring

### substring
Retorna uma parte da string entre os índices especificados.

~~~dart

String str = "Hello World";
print(str.substring(0, 5)); // "Hello"
~~~

### split
Divide a string em uma lista de substrings usando um delimitador.

~~~dart

String str = "Hello, World";
List<String> partes = str.split(",");
print(partes); // ["Hello", " World"]
~~~

## Métodos de Substituição

### replaceAll
Substitui todas as ocorrências de uma substring por outra substring.

~~~dart

String str = "Hello World";
print(str.replaceAll("o", "a")); // "Hella Warld"
~~~

### replaceFirst
Substitui a primeira ocorrência de uma substring por outra substring.

~~~dart

String str = "Hello World";
print(str.replaceFirst("o", "a")); // "Hella World"
~~~

### replaceRange
Substitui um intervalo específico de uma substring por outra substring.

~~~dart

String str = "Hello World";
print(str.replaceRange(6, 11, "Everyone")); // "Hello Everyone"
~~~

## Outros Métodos Úteis

### codeUnits
Retorna uma lista de unidades de código UTF-16 da string.

~~~dart

String str = "Hello";
print(str.codeUnits); // [72, 101, 108, 108, 111]
~~~

---

[Índex](../README.md)