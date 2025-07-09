# Semana 4: POO na Prática - Criando nossa Primeira Classe

Nesta semana, saímos da teoria para a prática! Vamos aprender a sintaxe para criar nossas próprias classes e objetos em Python, aplicando os conceitos que discutimos na introdução à Programação Orientada a Objetos.

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Utilizar a sintaxe `class` para definir uma classe em Python.
* Implementar o método construtor `__init__` para inicializar um objeto.
* Diferenciar os parâmetros de uma função dos atributos de uma instância (`self`).
* Criar métodos para definir os comportamentos de um objeto.
* Instanciar objetos a partir de uma classe e acessar seus atributos e métodos.

## 📖 Material de Estudo Principal

Todo o conteúdo aprofundado, com exemplos de código que você pode executar e modificar, está no notebook interativo da aula. Clique no link abaixo para abri-lo diretamente no Google Colab.

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-04/semana_4_classes_e_objetos.ipynb)**

---

## 💻 Exercício da Semana: Criando a Classe Aluno

Agora que aprendemos a criar classes, é hora de colocar a mão na massa. O objetivo deste exercício é criar uma classe para representar um `Aluno`, aplicando todos os conceitos vistos no material da semana.

### Instruções

1.  Crie um novo arquivo Python chamado `aluno.py`.
2.  Dentro deste arquivo, defina uma classe chamada `Aluno`.

3.  **Construtor (`__init__`):**
    * A classe deve ser inicializada com os atributos `nome` e `idade`.
    * Ela também deve ter um atributo chamado `notas`, que deve ser inicializado como uma **lista vazia** `[]`.

4.  **Métodos:**
    * Crie um método chamado `adicionar_nota(self, nota)`:
        * Este método deve receber uma `nota` (um número) como parâmetro.
        * Ele deve adicionar essa nota à lista `notas` do aluno.
    * Crie um método chamado `calcular_media(self)`:
        * Este método deve calcular a média de todas as notas que estão na lista `notas`.
        * **Importante:** Se a lista de notas estiver vazia, o método deve retornar `0` para evitar erros.
        * Ao final, o método deve **retornar** o valor da média calculada.

5.  **Código de Teste:**
    * No final do seu arquivo, fora da classe, crie um código para testar sua implementação:
        * Instancie um objeto da classe `Aluno` (ex: `aluno1 = Aluno("João", 16)`).
        * Use o método `adicionar_nota()` para adicionar pelo menos 3 notas a este aluno.
        * Chame o método `calcular_media()` e guarde o resultado em uma variável.
        * Use `print()` para exibir uma mensagem mostrando o nome do aluno e sua média final. Exemplo: `"A média final do aluno João é 8.5"`.

### Entrega

* Faça o upload do seu arquivo `aluno.py` completo na tarefa correspondente no **AVEA**.