# Semana 5: POO - Herança e a Magia da Reutilização

Olá! Nesta semana, vamos explorar um dos conceitos mais poderosos da Programação Orientada a Objetos: a **Herança**.

Depois de aprender a criar nossas próprias classes, vamos descobrir como podemos criar novas classes que "herdam" características e comportamentos de outras já existentes. Este é o segredo por trás da produtividade de frameworks como o Django, e dominá-lo vai nos poupar muito tempo e código!

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Definir o que é Herança e identificar a relação entre classe-pai e classe-filha.
* Implementar uma classe que herda de outra em Python.
* Especializar uma classe-filha, adicionando novos atributos e métodos.
* Utilizar a função `super()` para reaproveitar o construtor da classe-pai.
* Explicar como a Herança é aplicada nos Models e Views do Django.

## 📖 Material de Estudo Principal

Todo o conteúdo aprofundado, com o passo a passo de como implementar herança em Python e exemplos práticos, está no notebook interativo da aula. Clique no link abaixo para abri-lo diretamente no Google Colab.

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-05/aula_semana_05.ipynb)**

---

## 💻 Exercício da Semana: Sistema de Veículos com Herança

Nesta atividade, você irá modelar diferentes tipos de veículos usando os conceitos de Herança para evitar a repetição de código e criar uma estrutura organizada.

### Instruções

1.  Crie um novo arquivo Python chamado `veiculos.py`.

2.  **Classe-Pai (`Veiculo`):**
    * Crie uma classe chamada `Veiculo`.
    * No construtor `__init__`, ela deve receber os atributos `marca` e `modelo`.
    * Crie um método chamado `exibir_dados()` que imprime uma mensagem formatada com a marca e o modelo do veículo. Ex: `"Veículo: Ford Ka"`.

3.  **Primeira Classe-Filha (`Carro`):**
    * Crie uma classe chamada `Carro` que **herda** da classe `Veiculo`.
    * O construtor do `Carro` deve receber `marca`, `modelo` e `quantidade_portas`.
    * Utilize a função `super()` para chamar o construtor da classe-pai e inicializar a marca e o modelo.
    * O atributo `quantidade_portas` deve ser inicializado na própria classe `Carro`.

4.  **Segunda Classe-Filha (`Moto`):**
    * Crie uma classe chamada `Moto` que também **herda** de `Veiculo`.
    * O construtor da `Moto` deve receber `marca`, `modelo` e `cilindradas`.
    * Utilize `super()` de forma semelhante ao que foi feito na classe `Carro`.

5.  **Código de Teste:**
    * No final do seu arquivo, crie o código para testar sua implementação:
    * Instancie um objeto da classe `Carro` e um objeto da classe `Moto`, com dados de sua preferência.
    * Chame o método `exibir_dados()` para cada um dos objetos criados e veja se a saída está correta.

### Entrega

* Faça o upload do seu arquivo `veiculos.py` completo na tarefa correspondente no **AVEA**.