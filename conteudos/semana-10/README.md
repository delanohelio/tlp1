# Semana 10: Serializers - Os Tradutores da Nossa API

Olá, turma!

Na semana passada, criamos a base de dados da nossa aplicação com os Models do Django, definindo como um "Produto" deve ser. Agora, temos um desafio: como podemos "traduzir" um objeto `Produto` do nosso banco de dados para o formato JSON, que é a linguagem universal das APIs?

Nesta semana, vamos conhecer os **`Serializers`** do Django REST Framework. Eles são os componentes mágicos que fazem exatamente essa tradução, preparando nossos dados para viajar pela internet.

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Explicar o conceito de **Serialização** (Python -> JSON) e **Desserialização** (JSON -> Python).
* Criar um `ModelSerializer` para um Model existente.
* Utilizar a classe interna `Meta` para configurar o serializer.
* Especificar quais campos (`fields`) do Model devem ser incluídos na representação JSON.
* Testar o serializer no shell interativo do Django para converter um objeto em dados serializados.

## 📖 Material de Estudo Principal

O notebook da aula é um guia prático que mostra passo a passo como criar e testar seu primeiro serializer. Ele inclui testes no `shell` do Django para que você possa ver o resultado antes mesmo de ter uma API no ar.

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-10/aula_semana_10.ipynb)**

---

## 💻 Exercício da Semana: Criando o Serializer de Produto

O objetivo desta atividade é criar o "tradutor" para o `Model` de `Produto` que fizemos na aula passada.

### Instruções

1.  No seu projeto Django, dentro da sua app `api`, crie um novo arquivo chamado `serializers.py`. Se ele já existir, utilize-o.

2.  Neste arquivo, você deve:
    * Importar `serializers` do `rest_framework`.
    * Importar seu `Model` `Produto` do arquivo `api/models.py`.

3.  Crie uma classe chamada `ProdutoSerializer` que herda de `serializers.ModelSerializer`.

4.  Dentro da `ProdutoSerializer`, crie uma classe interna chamada `Meta`.

5.  Na classe `Meta`, configure duas coisas:
    * O `model` que este serializer irá representar (que é o `Produto`).
    * Os `fields` que você quer expor na API. Por enquanto, utilize a opção `fields = '__all__'` para incluir todos os campos do seu `Model` automaticamente.

### Entrega

* Faça o upload do seu arquivo `api/serializers.py` completo na tarefa correspondente no **AVEA**.