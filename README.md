# 🔤 Transformação de Nomes de Produtos com Método de Instância (Java)

Este projeto demonstra como utilizar a API de Streams em Java para transformar os nomes de uma lista de produtos em letras maiúsculas, 
usando uma referência a **método de instância**.

---

## 🚀 Objetivo

- Aplicar a transformação de nomes para letras maiúsculas usando método de instância da classe `Product`.
- Praticar o uso da interface funcional `Function` através de referência a método.
- Trabalhar com Streams API do Java 8+ para manipulação funcional de coleções.

---

## 🧩 Estrutura do Projeto

├── app/
│ └── Program.java // Classe principal
├── entities/
│ └── Product.java // Classe que representa um produto com método de instância para transformar nome
└── util/
├── UpperCaseName.java // (opcional, não usado diretamente neste projeto)
└── PriceUpdate.java // (opcional)

---

## 🔧 Como funciona

1. O programa cria uma lista de produtos com nome e preço.
2. Usa `Stream.map()` para transformar os nomes dos produtos em maiúsculas, chamando o método de instância `nonStaticUpperCaseName` em cada produto:
   ```java
   List<String> names = list.stream()
                            .map(Product::nonStaticUpperCaseName)
                            .collect(Collectors.toList());
    Imprime os nomes convertidos no console.
   

📌 Exemplo de saída

TV
MOUSE
TABLET
HD CASE

📚 Conceitos utilizados

    Java 8+

    Programação funcional

    API de Streams (stream(), map(), collect())

    Referência a método de instância (ClassName::methodName)

    Encapsulamento e métodos utilitários na classe Product

▶️ Como executar
Requisitos:

    JDK 8 ou superior

    IDE Java ou terminal

Executar via terminal:

javac app/Program.java
java app.Program



