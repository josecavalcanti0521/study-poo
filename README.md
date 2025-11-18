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

## Applets

O que é um Applet? Um Applet é um programa Java pequeno que pode ser embutido em uma página web (HTML) e executado dentro de um navegador.

Exemplos:

- import javax.swing.*; // pacote gráfico swing
- import java.awt.Graphics; // Pacote gráfico awt : Graphics
 
 O método public void paint (Graphics g) {} o g se diz a respeito a uma instância da classe Graphics, onde esse g possibilitará a utilização dos métodos dessa classe.

 No HTML deve ser refenciar a classe que está utilizando o Applet com o arquivo .class.

 <applet code="AppletCliente.class" width=800 height=600>

 Logo após o appletviewer executa o .HTML que referencia o arquivo .class que é um Applet.

 Métodos da biblioteca:

- public void init () - Chamado na 1ª execução do
applet
- public void start () - Chamado após o método init ou
quando o usuário retorna a página do applet
- public void paint () - Chamado após o método init e o
do método start. Chamado também automaticamente
quando o applet é repintado.
- public void stop () - Chamado quando o applet pára
a execução.
= public void destroy () - Chamado quando o applet
está sendo removido da memória.