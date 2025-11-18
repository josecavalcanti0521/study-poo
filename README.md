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

## Exceções

***O que são as exceções:***
As exceções são maneiras que o programador tem de tratar o erro que pode acontecer durante a execução do programa, como por exemplo uma divisão por 0, etc. Pode ser utilizadas as exceções predefinidas do Java ou criar as próprias exceções
- Claros 
- Robustos 
- Tolerantes a falhas

***As palavras chave são:***
- Throws Exception: deixa o codigo sobre o aviso que pode dar errado e gerar uma exceção
- Try: envolve o bloco que pode pegar a exceção 
- Catch: captura e trata uma exceção
- Finally: código sempre executado independentemente de uma exceção ocorrer

## Concorrência ou Multithreading

Multithreading é o ato de você dividir os processos em threads, onde cada thread é única e independente. Como por exemplo, um usuário em um site de e-commerce, cada usuário é um thread no computador que está rodando a aplicação. Trazendo a ideia de execução simultânea.

Métodos:

- public void run() -> executar uma thread
- void start () - método que dispara a thread, chamando o
método run ()
- void sleep (int miliseconds) - método que especifica
quanto tempo (em milisegundo) a thread deve “dormir”
- boolean interrupt () - método que interrompe a thread
- boolean isInterrupted () - método que retorna se a
thread está ou não interrompida

### Sincronização (synchronized)

Um dos conceitos mais importantes em Multithreading é a sincronização.
Como as threads compartilham memória, é preciso proteger dados críticos. O Java usa a palavra-chave synchronized para garantir que apenas uma thread por vez possa acessar um bloco de código ou método específico.

Isso resolve o problema de condição de corrida, onde o resultado do programa depende da ordem aleatória em que as threads acessam e modificam os dados.