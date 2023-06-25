## Atividades Práticas Integradoras &emsp;&emsp; &emsp;  <a href='https://github.com/4chan/4chan-API' target="_blank"><img alt='Github' src='https://img.shields.io/badge/4chan_API-100000?style=plastic&logo=Github&logoColor=white&labelColor=BABABA&color=black'/></a> <a href='https://ufmg.br/cursos/graduacao/2358/91199/60539' target="_blank"><img alt='Google Scholar' src='https://img.shields.io/badge/Atividades_Práticas Integradoras (UFMG)-100000?style=plastic&logo=Google Scholar&logoColor=white&labelColor=2F00B0&color=2F00B0'/></a>

#### Disciplina do curso de Sistemas de Informação - DCC/UFMG
***
Este script é destinado à **coleta** e **estruturação de dados** do fórum online 4chan, visando a construção de **datasets** para análise em trabalhos posteriores.<br />

**Aluno**: Diego Tomaz<br />
**Orientadores**: Martín G. Ravetti e Allana T. Bastos <br />
 
A priori este script objetivará a coleta de dados apenas da board /pol/, dado a natureza do estudo que consumirá esses datasets. <br />

### Regras da API: 
 1. Uma requisição por segundo; 
 2. Atualização do thread deve ser definida
    para um mínimo de 10 segundos, de preferência mais alto; 
 3. Uso do 'If-Modified-Since' nas requisições para não solicitar dados de
    threads sem atualização.

### Estrutura dos dados (.csv)
`thread_no:` número que identifica unicamente uma thread no fórum. Uma thread é basicamente um tópico de discussão separado;<br>
`post_no:` número que identifica unicamente uma postagem dentro de uma thread. Cada postagem é uma contribuição separada para a discussão da thread;<br>
`comment:` texto da postagem. É a conteúdo real que alguém fez para a discussão na thread;<br>
`image_replies:` número de respostas com imagens que a postagem recebeu; <br>
`timestamp:` marca de tempo de quando a postagem foi feita. Está no formato de um timestamp UNIX, que é o número de segundos desde 01 de janeiro de 1970;<br>
`reply_to:` número da postagem à qual a postagem atual está respondendo dentro da thread;<br>
`image_id:` dentificador único da imagem associada à postagem. É composto pelo número da thread, número da postagem e a extensão do arquivo de imagem. Se a postagem não tiver uma imagem, esse campo não será incluído.
