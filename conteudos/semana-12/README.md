# Semana 12: Detalhando a Informação - Endpoint de Detalhe

Olá, turma!

Na semana passada, criamos nosso primeiro endpoint para listar todos os produtos. Agora, vamos adicionar a funcionalidade de visualizar um item específico.

Nesta aula, vamos criar o endpoint de **detalhe**, que permitirá acessar um produto através de seu ID (ex: `/api/produtos/1/`), utilizando URLs dinâmicas. Com isso, completaremos as operações de leitura da nossa API.

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Utilizar a `View` genérica `RetrieveAPIView` para buscar e exibir um único objeto.
* Entender e implementar padrões de URL dinâmicos para capturar parâmetros (ex: `<int:pk>`).
* Adicionar uma nova rota ao arquivo `urls.py` da aplicação para o endpoint de detalhe.
* Testar o novo endpoint usando a `Browsable API` do DRF.
* Reforçar a conexão entre a URL, a View, o Model e o Serializer no fluxo de uma requisição.

## 📖 Material de Estudo Principal

O notebook da aula guia você na adição da nova view de detalhe e na configuração da URL dinâmica correspondente. Siga os passos com atenção!

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-12/aula_semana_12.ipynb)**

---

## 💻 Exercício da Semana: Criando o Endpoint de Detalhe

O objetivo desta atividade é colocar em prática a criação de uma `View` de detalhe e a configuração de uma `URL` dinâmica.

### Instruções

1.  Siga todos os passos do notebook da aula para adicionar a `View` `ProdutoDetail` ao seu arquivo `api/views.py`.
2.  Atualize o arquivo `api/urls.py` para incluir a nova rota dinâmica para a view de detalhe.
3.  Inicie o servidor, adicione alguns produtos pelo Django Admin (se ainda não tiver) e teste ambos os endpoints (`/api/produtos/` e `/api/produtos/<id>/`) para garantir que estão funcionando.

### Entrega

Para comprovar a conclusão da atividade, você deve entregar **três capturas de tela (prints)**:

1.  **Print 1:** Uma captura de tela mostrando o código completo do seu arquivo `api/views.py`, com as **duas** classes de view (`ProdutoList` e `ProdutoDetail`).
2.  **Print 2:** Uma captura de tela mostrando o código completo do seu arquivo `api/urls.py`, com as **duas** rotas configuradas.
3.  **Print 3:** Uma captura de tela da janela do seu navegador mostrando a `Browsable API` do DRF para o endpoint de **detalhe** de um produto específico (ex: `http://127.0.0.1:8000/api/produtos/1/`).

Crie um documento de texto ou PDF, cole os **três prints** solicitados e envie o arquivo na tarefa correspondente no **AVEA**.
