# Estudos de Teoria da Segunda Unidade

## Interface

***O que é uma interface?***
Basicamente uma interface firma um contrato com uma classe, pois a classe obrigatoriamente deverá implementar os métodos definidos na interface, com a palavra reservada "implements". O Java utiliza interfaces para ter essa ideia de herança multipla, pois uma classe pode implementar mais de uma interface, lebrando que no Java 6 uma interface somente tem métodos e não atributos.


## Pacotes 

***O que são os pacotes?***
Pacotes contém um conjunto de classes encapsuladas, que possibilitam uma reutilização de software. Basicamente se comportam como uma biblioteca. Possuindo as seguintes palavras reservadas: package e o import.

**package:** declara a qual pacote essa classe pertence 
Ex. package meu.projeto.utilitarios; a minha classe pertence a esse pacote   
**import:** referenciar classes de outros pacotes sem usar seus nomes completos 
Ex. import java.util.Scanner; você pode usar o Scanner sem ter que chamar todo o nome dele a cada uso
