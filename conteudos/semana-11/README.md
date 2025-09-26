# Semana 11: Dando Vida à API - Views e o Primeiro Endpoint

Olá, turma!

Chegou o momento de conectar todas as peças! Nas últimas semanas, construímos nossa base de dados com `Models` e criamos o "tradutor" com `Serializers`. Nesta aula, vamos usar as **`Views`** e as **`URLs`** para finalmente criar nosso primeiro endpoint de API.

Ao final desta aula, você terá uma URL funcional que retorna uma lista de produtos do seu banco de dados, formatada em JSON, e acessível pelo navegador!

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Explicar o papel de uma `View` no ciclo de requisição-resposta de uma API.
* Utilizar a `View` genérica `ListAPIView` para listar todos os objetos de um `Model`.
* Configurar os atributos `queryset` e `serializer_class` em uma `View`.
* Mapear uma URL para uma `View` usando o sistema de roteamento do Django (`urls.py`).
* Diferenciar e conectar os arquivos de URL do projeto e da app.
* Testar um endpoint funcional através do navegador e da `Browsable API` do DRF.

## 📖 Material de Estudo Principal

O notebook da aula é um guia prático que une todos os conceitos que aprendemos. Siga cada passo com atenção para criar seu primeiro endpoint!

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-11/aula_semana_11.ipynb)**

---

## 💻 Exercício da Semana: Publicando seu Primeiro Endpoint

O objetivo desta atividade é colocar em prática a criação de uma `View` e a configuração de uma `URL`, resultando em um endpoint de listagem funcional.

### Instruções

1.  Siga todos os passos do notebook da aula para criar a `View` `ProdutoList` no arquivo `api/views.py`.
2.  Crie o arquivo `api/urls.py` e configure a rota para a sua `View`, como mostrado no guia.
3.  Modifique o arquivo principal `meuprojeto/urls.py` para incluir as rotas da sua `api`.
4.  Inicie o servidor (`python manage.py runserver`) e acesse o endpoint no seu navegador para garantir que tudo está funcionando.

### Entrega

Para comprovar a conclusão da atividade, você deve entregar **três capturas de tela (prints)**:

1.  **Print 1:** Uma captura de tela mostrando o código completo do seu arquivo `api/views.py`.
2.  **Print 2:** Uma captura de tela mostrando o código completo do seu arquivo `api/urls.py`.
3.  **Print 3:** Uma captura de tela da janela do seu navegador mostrando a `Browsable API` do DRF com a lista de produtos no endereço `http://127.0.0.1:8000/api/produtos/`.

Crie um documento de texto ou PDF, cole os **três prints** solicitados e envie o arquivo na tarefa correspondente no **AVEA**.
