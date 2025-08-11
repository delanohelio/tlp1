# Semana 8: Mão na Massa! Introdução ao Django

Olá, pessoal!

Chegou o momento que todos esperavam! Depois de construir uma base sólida em POO, HTTP e APIs, vamos finalmente começar a usar uma das ferramentas mais poderosas do mundo Python para desenvolvimento web: o framework **Django**.

Nesta semana, nosso objetivo é preparar nosso ambiente de desenvolvimento, instalar o Django, criar nosso primeiro projeto e entender a estrutura de arquivos que ele gera para nós. Vamos ligar o motor do nosso foguete!

---

## 🎯 Objetivos de Aprendizagem

Ao final desta semana, você será capaz de:

* Explicar o que é um ambiente virtual (`venv`) e por que ele é essencial para projetos Python.
* Instalar o Django em um ambiente virtual usando o `pip`.
* Utilizar o comando `django-admin startproject` para criar a estrutura de um novo projeto.
* Descrever a função dos arquivos principais gerados (`manage.py`, `settings.py`, `urls.py`).
* Iniciar o servidor de desenvolvimento do Django com o comando `runserver`.
* Visualizar a página de boas-vindas do Django no navegador.

## 📖 Material de Estudo Principal

O notebook da aula contém o **passo a passo detalhado**, com todos os comandos que você precisa executar no seu terminal para configurar o ambiente e criar seu projeto. Siga-o com muita atenção!

**[➡️ Abrir o notebook da aula no Google Colab](https://colab.research.google.com/github/delanohelio/tlp1/blob/main/conteudos/semana-08/aula_semana_08.ipynb)**

---

## 💻 Exercício da Semana: Criando seu Primeiro Projeto Django

O objetivo desta atividade é garantir que você consiga configurar seu ambiente de desenvolvimento local corretamente. Esta é a base para todas as nossas próximas aulas práticas.

### Instruções

Siga os passos abaixo no terminal do seu computador:

1.  **Crie a Pasta do Projeto:** Em um local de sua preferência (Ex: `Documentos/`), crie uma nova pasta para a nossa disciplina. Ex: `mkdir ltp1_projetos`. Acesse essa pasta: `cd ltp1_projetos`.

2.  **Crie o Ambiente Virtual:** Dentro da pasta `ltp1_projetos`, crie um ambiente virtual.
    * No Windows: `python -m venv venv`
    * No macOS/Linux: `python3 -m venv venv`

3.  **Ative o Ambiente Virtual:**
    * No Windows: `venv\\Scripts\\activate`
    * No macOS/Linux: `source venv/bin/activate`
    * (Você saberá que funcionou pois `(venv)` aparecerá no início da linha do seu terminal).

4.  **Instale o Django:** Com o ambiente ativo, execute o comando: `pip install django`

5.  **Crie o Projeto:** Agora, crie um projeto Django chamado `meuprojeto`.
    * `django-admin startproject meuprojeto .` (Não esqueça o ponto `.` no final!)

6.  **Inicie o Servidor:** Execute o comando para ligar o servidor de desenvolvimento.
    * `python manage.py runserver`

7.  **Verifique no Navegador:** Abra seu navegador e acesse o endereço `http://127.0.0.1:8000/`. Você deverá ver a página de sucesso do Django.

### Entrega

Para comprovar a conclusão da atividade, você deve entregar **duas capturas de tela (prints)**:

1.  **Print 1:** Uma captura de tela do seu editor de código (VS Code) mostrando a estrutura de pastas do `meuprojeto` que foi criada. A imagem deve mostrar claramente a pasta do ambiente `venv` e os arquivos como `manage.py`.
2.  **Print 2:** Uma captura de tela do seu navegador mostrando a página de boas-vindas do Django com a mensagem "The install worked successfully! Congratulations!".

Crie um documento de texto ou PDF, cole os dois prints e envie o arquivo na tarefa correspondente no **AVEA**.