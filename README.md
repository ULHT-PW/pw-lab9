**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

# Lab 9: Portfolio II ⛅

### Objetivo 

* Finalizar e aprimorar os requisitos do Lab. 8.
* Recolher todos os conteúdos necessários, organizados numa pasta e em ficheiros de texto, tal como indicado no Lab. 8.
* desenhar o diagrama entidade relação da base de dados a construir no Lab. 10


### Recomendações
* leia uma vez o enunciado. Este detalha todos os passos e fornece o código necessário, sendo rápida a sua realização.
* se tiver dúvidas, consulte os [slides](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-04-django-01.pptx) e a documentação do [djangoproject](https://www.djangoproject.com/)
* familiarize-se e use o [glossario](https://moodle.ensinolusofona.pt/pluginfile.php/353336/mod_resource/content/1/PW_glossario.pdf) que terão disponivel no exame.


## 0. Primeiros passos 👶
Trabalhe a partir do seu projeto criado no Lab 8. 
1. se o tiver no computador onde odesenvolveu, basta ativar o ambiente virtual com "pipenv shell".
2. Se estiver a trabalhar no projeto noutro computador, deve 
   * instalar os modulos necessarios, com o compando `pipenv install`
   * ativar o ambiente virtual, com `pipenv shell`  

## 1. Aprimore a sua aplicação ✨
4. Este será o seu portfolio, carta de apresentação sua na internet muito valorizada no mundo do trabalho! Por isso, esmere-se, e abrir-lhe-á oportunidades de emprego muitas na medida do que se aplicar neste projeto. 
* Releia o enunciado do Lab. 8 com atenção e garanta que implementou tudo, e tem tudo a funcionar devidamente
* Esmere-se no layout, garantindo que tem um aspecto profissional e aplica tecnicas modernas de CSS.
* Várias páginas irão apresentar um conjunto de items (cadeiras, projetos, TFCs), com um titulo, imagem, texto e mais alguns atributos. Desenhe o layout destes items independentes / tipo postais, como feito no laboratório anterior lab.5. Crie elementos para cada página, com conteúdos inventados para já. 

## 2. Blog

* Implemente um blog, que permite realizar posts. Siga os passos da aplicação [Tarefas]() desenvolvida na aula, disponível com todos os detalhes (e estilização CSS que não cheguei a fazer por falta de tempo)
* **Blog**. Post tem atributos autor, data, título e descrição e eventualmente um link (para projeto, página do seu portfolio) e foto. deverá ter pelo menos 5 posts de outros colegas seus a comentar que gostaram de fazer um determinado projeto consigo, ou de certo trabalho que você fez, ou que é um bom colega para estudar



## 2. Quizz sobre programação Web

* Conceba um Quizz sobre programação Web, em especial sobre aspectos falados na sua secção sobre Programação Web (veja em baixo). Siga as indicações do [lab 3](https://github.com/ULHT-PW/pw-lab3#3-p%C3%A1gina-com-quizz-), tentando ter variedade no tipos de perguntas. Deverá também recolher o nome da pessoa que responde.
* Crie no models.py uma classe para guardar os resultados das perguntas, relativo às pessoas que responderem.
* Crie um ficheiro no forms.py para construir um formulário com base na tabela (veja a aplicação desenvolvida na aula). Explore labels, widgets e help-texts.
* Quando o Quizz é submetido, deverá apresentar o resultado com uma cotação/nota/qualificação por pergunta e nota global. Para tal, deverá criar uma função na qual deverá analisar as respostas e atribuir cotações, retornando uma página de resultados. 
* Crie um gráfico de barras para mostrar os resultados do Quizz. 
   * Explore o [Matplotlib](https://moodle.ensinolusofona.pt/pluginfile.php/318343/mod_label/intro/pw-03-python-04-matplotlib.pdf?#page=20) para criar um gráfico de barras e gravá-lo. 
   * Na view do quizz, chame uma função cria_resultados. Esta deverá obter da base de dados todas as respostas ao quizz (nome e pontuação), criar um grafico de barras e guardá-lo na pasta portfolio\static\images. Os resultados devem ser mostrados no topo do Quizz, na sua apresentação, indicando também quem está em primeiro lugar.


## 2. Comentários
* Crie um formulário para recolher comentários sobre o website, avaliando 10 critérios. Listam-se em baixo alguns padrões intelectuais do pensamento crítico: 
      * clareza (compreensível, em que o significado pode ser identificado sem que haja confusão ou ambiguidade.)
      * rigor (livre de erros)
      * precisão (exato, segundo o nível necessário do pormenor)
      * profundidade (contém complexidades e múltiplas inter-relações)
      * amplitude (que abrange diferentes aspectos, pontos de vista, pespectivas)
      * lógica (em que as partes fazem sentido num todo, sem contradições: faz sentido no conjunto, provém de evidências)
      * significância (focado no importante, não trivial)
      * originalidade (criativo e original)
   * Para tal, crie uma tabela em Models utilize elementos `input` com atributos `range`, `checkbox` e `radio`. Deverá igualmente ter um elemento `textarea` que permita submeter sugestões de melhoria.

* Quando desenvolver o *back-end*, será capaz de processar estes dados introduzidos por
utilizadores e será capaz de fazer uma análise do seu website assim como uma visão crítica deste. 

# Ready... GO! 🏁
1. Lance a aplicação com o comando `python manage.py runserver` e verifique que consegue visualizar corretamente a aplicação que fez. 




## 2. Diagrama Entidade Relação 🛢

* Desenhe o Diagrama Entidade Relação com uma ferramenta a seu gosto (por exemplo [draw.io](draw.io)). 
* Neste laboratório concentrar-se-á na modelação e só no Lab. 10 irá implementar a base de dados. Deverá identificar todas as classes, atributos e relações (1:1, 1:N e N:N).
* Para construir o DER leia com atenção os requisitos da secção 3 onde se detalham muitas das tabelas e atributos que irá ter, assim como relações.
* Este DER deverá ser apresentado 


## 3. Recolha de Conteúdos 📚

* Durante esta semana deverá recolher **todo o material em baixo**. Organize-o e guarde-o numa pasta. No Lab 10, após construir a base de dados, irá inserir os conteúdos. Atenção que foram adicionados mais alguns intems em relação à estrutura apresentada no Lab. 8, secção 10. Alterou-se tambem o aninhamento de Licenciatura dentro de Educação.

* **Hero Page**
  * Redija um texto de apresentação, (que irá colocar na HeroPage no segundo elemento, ver indicação no Lab. 8) que fale de:
    * de motivações para escolher o seu curso, 
    * daquilo que mais tem gostado de aprender no curso,
    * de espectativas do que gostaria de fazer quando acabar o curso. 
    * de hobbies

* **Educação**
   * educação, listar Formação, com campos curso, local, período logotipo da instituição
      * cursos superior
      * escolas no secundário
      * certificados
   * licenciatura, pagina que apresenta a lista de cadeiras do curso, organizada por semestre e anos. Quando clicada uma cadeira, aparece informação relativamente a: nome, ano, semestre, ECTS, ano letivo frequentado, topicos abordados, ranking de 1 a 5 estrelas (indicando se gostou ou não), professores (da classe Pessoa com campos nome e link para a sua pagina da lusofona e no linkedin), link para página da cadeira (se existir), lista de projetos realizados (classe projeto)
   * Aptidões e competências pessoais (com atributos titulo, descrição curta, lista de projetos (Projeto) realizados onde foi aplicada essa competência caso se aplique, lista de disciplinas (Disciplina) onde foi trabalhada essa competência caso se aplique)
         * [Técnicas]( https://www.e-konomista.pt/competencias-tecnicas/): 
         * linguagens de programação ou tecnologias, relatórios word, apresentações powerpoint, realização de videos, protótipos
         * [Organizativas]( https://www.e-konomista.pt/competencias-de-organizacao/)
         * [Sociais](https://www.e-konomista.pt/aptidoes-e-competencias-sociais)
         * Linguísticas. lista de linguas estrangeiras faladas, com indicação de nível (proficiente, independente ou elementar), e referencia se existir a certificação obtida ou outra explicação (lingua materna, viveu noutro país)
   * interesses (com atributos titulo, descrição, fotografia e link (e.g., clube de fotografia) 
         * outras atividades
         * desporto
         * hobbies
         * voluntariado

* **Projetos**
   * realizados por mim: lista de projetos realizados, com atributos: titulo, descrição até 500 carateres, imagem, ano de realização, cadeira (classe Cadeira, caso tenha sido projeto associado a uma cadeira), participantes (da classe Pessoa, da classe Pessoa com atributos nome e link para a sua pagina no linkedin, e link para a aplicação portfolio do projeto PW), link para repositorio GitHub, link para video no youtube, tecnologias usadas, competencias (classe Competencia)
   * trabalhos de fim de curso: lista de 6 Trabalhos finais de Curso (TFCs) de anos passados realizados por colegas seus que achou interessantes, onde TFC tem atributos: titulo, autor (multiplos), orientador (multiplos), ano de realização, sumário, resumo até 500 carateres, link para relatório, links para repositório github e vídeo no Youtube, se existentes. Será facultada uma pasta com relatórios de TFC dos últimos anos para consultar e escolher.

* **Programação Web**
   * Tecnologias: Falar das seguintes Tecnologias, com os atributos: nome (por extenso), acrónimo (caso exista, e.g., CSS para Cascade Style Sheet), ano de criação, criador, logotipo, link para site oficial, descrição das principais características. 
         * Back-end: Laravel, ASP.NET, Spring MVC, Express, Django
         * Front-end: Angular, React, Vue, Svelte
         * Outras: WordPress, OutSystems, Weebly, Wix
   * Laboratórios: página que lista links para os laboratórios realizados na disciplina de PW, com o título e descrição dos tópicos abordados
   * Notícias: listagem de 10 noticias sobre artigos do medium.com que tenha gostado, com campos: título, 3 linhas de texto, imagem e link
   * exemplos de técnicas e efeitos que gosta, sites que gosta e de sites que acha maus, tendencias modernas de programação Web, aspectos obsoletos

* **Blog**. Post tem atributos autor, data, título e descrição e eventualmente um link (para projeto, página do seu portfolio) e foto. deverá ter pelo menos 5 posts de outros colegas seus a comentar que gostaram de fazer um determinado projeto consigo, ou de certo trabalho que você fez, ou que é um bom colega para estudar

* **Sobre este website**, informação sobre este website, incluindo
   * Estrutura do website: com mapa do site
   * Descrição da base de dados e sua modelação, incluindo o DER e explicação de principais relações.
   * lista de tecnologias usadas na criação do website: HTML, CSS, Python, Django, Heroku, JavaScript). Tecnologia terá os seguintes atributos: nome (por extenso), acrónimo (caso exista, e.g., CSS para Cascade Style Sheet), ano de criação, criador, logotipo, imagem exemplificativa (excerto de código, e.g.) link para site oficial, descrição do que é e onde & como foi usado. 
   * lista de padrões usados: padrão arquitetural cliente-servidor HTTP, padrão de software MVC, padrão de comunicação assíncrona (AJAX) 
   * Comentários: para recolher opiniões sobre o seu website, avaliando 10 critérios, tal como descrito na secção acima.

* **Contacto**
   * links para a sua conta linkedin. se não tiver, crie. Adicione à sua conta de colegas seus, amigos e professores e adira a grupos de interesse na sua área (DEISI)
   * link para o seu github
   * link para conta Instagram, facebook
   * nome da cidade onde vive
   * facebook, instagram

* **Rodapé**
   * link para Mapa do site
   * contacto
   * nome do autor
   * ano
   * universidade
   * logotipo



## Contacto 🦸🏻‍♂️  
1. Deverá criar uma página com um formulário de contacto. Quando submetido, os dados deveão ficar guardados na base de dados. Deverá pedir em especial o email e guardá-lo num [campo adequado](https://docs.djangoproject.com/en/3.2/ref/models/fields/#emailfield). 
1. Deverá ser possível fazer operações CRUD sobre estes dados (listar, editar e apagar contactos).
1. No próximo lab configuraremos estes aspectos para que estejam disponíveis apenas para utilizadores autenticados.

## Quizz ❓
1. Crie um Quizz com no mínimo 10 perguntas sobre o tópico do seu projeto. Pode integrá-lo como uma nova app, mas usando o mesmo layout, e estando interligado pelo menu.
1. Siga as indicações do [lab 3](https://github.com/ULHT-PW-2020-21/pw-lab3#2-p%C3%A1gina-com-quizz) tentando ter alguma variedade de tipos de perguntas. 
2. Crie no model uma classe para guardar o Quizz
3. Crie um form para incluir no formulário informação necessário sobre o Quizz. Explore labels, widgets e help-texts.
4. Quando o Quizz é submetido, deverá apresentar o resultado com uma cotação/nota/qualificação por pergunta e nota global. Para tal, deverá criar uma função na qual deverá analisar as respostas e atribuir cotações, retornando uma página de resultados. 
5. Os resultados do Quizz deverão ficar guardados numa tabela, na base de dados, um registo por pessoa que responde. Esta irá ser associada a um registo, que implementaremos no próximo laboratorio.
6. Utilize graficos para mostrar os resultados. Explore o matplotlib (slides disponibilizados). 

# Comentários 😃
8. Criar uma página comentários sobre o site, como especificado no [lab. 3](https://github.com/ULHT-PW-2020-21/pw-lab3#3-p%C3%A1gina-coment%C3%A1rios). 
9. Considerando que irá receber muitas avaliações, guarde os dados numa base de dados.
10. Mostre os resultados recorrendo a gráficos criados com o matplotlib. Para  


# Ready... GO! 🏁
1. Lance a aplicação com o comando `python manage.py runserver` e verifique que consegue visualizar corretamente a aplicação que fez. 



## 8. Portfolio no Heroku 🌤️
* Crie um repositório GitHub para o seu projeto
* Crie outro repositório com o material que recolheu

## 4. Submissão

* submeta no formulário disponivel no Moodle o link para os 2 repositórios e o link para a plicação Heroku.

