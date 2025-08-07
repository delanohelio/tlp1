# Semana 7: APIs, REST e JSON - A Linguagem das Aplicações Modernas

Olá, turma!

Na semana passada, aprendemos o "idioma" da web, o protocolo HTTP. Agora, vamos aprender a organizar a "conversa" de uma forma padronizada e eficiente que permite que diferentes sistemas interajam de forma inteligente.

Nesta semana, vamos finalmente definir o que é uma **API**, entender os princípios do padrão **REST** que domina o mercado e conhecer o formato de dados **JSON**, que é o "RG" dos nossos objetos na internet.

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Definir o que é uma API (Application Programming Interface) e qual seu propósito.
* Explicar o que significa a arquitetura REST (Representational State Transfer).
* Descrever a relação entre Recursos, Endpoints (URIs) e os Métodos HTTP.
* Identificar a estrutura e a sintaxe do formato JSON (JavaScript Object Notation).
* Analisar uma requisição a uma API pública e interpretar sua resposta JSON.

## 📖 Material de Estudo Principal

Todo o material completo, com exemplos claros de como uma API REST funciona e como os dados são estruturados em JSON, está no notebook da aula. Acesse pelo link abaixo para abrir diretamente no Google Colab.

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-07/aula_semana_07.ipynb)**

---

## 💻 Exercício da Semana: Explorando a API DummyJSON

Nesta atividade, vamos interagir com uma API real e pública para ver na prática os conceitos que aprendemos. Usaremos a API **DummyJSON**, que fornece dados fictícios de "to-dos" (tarefas a fazer).

### Instruções

1.  **Acesse a API pelo Navegador:** Abra uma nova aba no seu navegador e acesse o seguinte link. Ele faz uma requisição para a API buscando por uma lista de tarefas.
    `https://dummyjson.com/todos`

2.  **Analise a Resposta:** Você verá uma resposta no formato JSON diretamente na sua tela, contendo uma lista de tarefas.

3.  **Responda as Perguntas:** Em um arquivo de texto, responda às seguintes perguntas com base na sua interação com a API.

    * **a)** Qual foi o **Endpoint (URI)** completo que você usou para fazer a requisição?
    * **b)** Qual **Método HTTP** o seu navegador usou para fazer essa requisição? (Dica: quando você digita um endereço na barra do navegador, qual é o método padrão?).
    * **c)** A resposta JSON que você recebeu tem uma chave principal chamada `"todos"`. Qual é o tipo de dado associado a essa chave (Ex: texto, número, lista, objeto)?
    * **d)** Dentro da lista de "todos", olhe para o **primeiro** item da lista. Qual é o valor da chave `"todo"` neste primeiro item?
    * **e)** Ainda no primeiro item da lista, qual é o valor associado à chave `"completed"`?

### Entrega

* Crie um arquivo de texto (`.txt`) com as respostas para as cinco perguntas (a, b, c, d, e).
* Faça o upload deste arquivo na tarefa correspondente no **AVEA**.