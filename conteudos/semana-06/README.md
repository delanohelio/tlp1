# Semana 6: Onde Nossas APIs Vão Morar - A Web e o Protocolo HTTP

Olá, pessoal!

Até agora, focamos em como organizar nosso código em Python usando a Programação Orientada a Objetos. Criamos "moldes" (classes) e "objetos" que vivem dentro do nosso programa. Mas, como fazemos para que um programa em um computador se comunique com outro do outro lado do mundo?

Nesta semana, faremos a ponte entre a programação e a internet. Vamos desvendar os conceitos fundamentais da web que tornam as APIs possíveis: o modelo **Cliente-Servidor** e o protocolo **HTTP**.

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Diferenciar o papel de um **Cliente** (como seu navegador) e de um **Servidor**.
* Explicar o que é o protocolo HTTP e qual a sua finalidade na comunicação web.
* Descrever as partes de uma requisição HTTP (método, URL, cabeçalhos, corpo).
* Listar e explicar os principais métodos (verbos) HTTP: `GET`, `POST`, `PUT` e `DELETE`.
* Entender o significado dos principais Códigos de Status HTTP (ex: 200 OK, 404 Not Found, 500 Internal Server Error).

## 📖 Material de Estudo Principal

Todo o conteúdo teórico, com analogias e diagramas para facilitar o entendimento, está no notebook da aula. Acesse pelo link abaixo para abrir diretamente no Google Colab.

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-06/aula_semana_06.ipynb)**

---

## 💻 Exercício da Semana: Analisando uma Requisição Web

Nesta semana, nossa atividade será prática, mas sem escrever código. Vamos usar as ferramentas do nosso próprio navegador para investigar como a web funciona por baixo dos panos.

### Instruções

1.  Abra o navegador Google Chrome (ou Firefox).
2.  Acesse um site de sua preferência (ex: `https://www.ifpe.edu.br`).
3.  Abra as **Ferramentas de Desenvolvedor** pressionando a tecla `F12` (ou `Ctrl+Shift+I` no Windows/Linux, `Cmd+Option+I` no Mac).
4.  Com as ferramentas abertas, clique na aba **"Rede"** (ou "Network").
5.  **Recarregue a página** (pressionando `F5` ou no botão de recarregar do navegador). Você verá uma lista de todas as requisições que a página fez.
6.  Clique na **primeira requisição** da lista, que geralmente corresponde ao documento principal da página (ex: `www.ifpe.edu.br`).
7.  Com essa requisição selecionada, uma nova janela de detalhes se abrirá. Investigue e responda às seguintes perguntas em um arquivo de texto:
    * **a)** Qual foi a **URL da Requisição** (Request URL)?
    * **b)** Qual foi o **Método da Requisição** (Request Method)?
    * **c)** Qual foi o **Código de Status** da resposta (Status Code)? O que esse código significa?
    * **d)** Na aba **"Cabeçalhos"** (Headers) da resposta, encontre o valor de `Content-Type`. Qual tipo de conteúdo o servidor retornou?

### Entrega

* Crie um arquivo de texto (`.txt`) com as respostas para as quatro perguntas (a, b, c, d).
* Faça o upload deste arquivo na tarefa correspondente no **AVEA**.