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
   * ativaro ambiente virtual, com `pipenv shell`  


## 1. Aprimore a sua aplicação ✨
4. Este será o seu portfolio, carta de apresentação sua na internet muito valorizada no mundo do trabalho! Por isso, esmere-se, e abrir-lhe-á oportunidades de emprego muitas na medida do que se aplicar neste projeto. 
* Releia o enunciado do Lab. 8 com atenção e garanta que implementou tudo, e tem tudo a funcionar devidamente
* Esmere-se no layout, garantindo que tem um aspecto profissional e aplica tecnicas modernas de CSS.
* Cada página irá listar um conjunto de items (cadeiras, projetos, TFCs) que têmassociados um titulo, imagem, texto e mais alguns atributos. Pense num layout de items independentes / tipo postais, como feito no laboratório anterior lab.5. Crie desde já elementos para cada página, com conteúdos inventados para já. 
* Garanta que ficam devidamente integrados os laboratórios feitos sobre HTML e JS, realizados anteriormente. Pense numa forma deficarem integrados no seu portfolio.

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


## 4. Submissão

* Crie um repositório GitHub para o seu projeto
* submeta o link para este no formulário disponivel no Moodle.
