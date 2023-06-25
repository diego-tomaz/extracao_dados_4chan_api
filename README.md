## Atividades Práticas Integradoras &emsp; <a href='https://github.com/4chan/4chan-API' target="_blank"><img alt='Github' src='https://img.shields.io/badge/4chan_API-100000?style=plastic&logo=Github&logoColor=white&labelColor=BABABA&color=black'/></a> <a href='https://ufmg.br/cursos/graduacao/2358/91199/60539' target="_blank"><img alt='Google Scholar' src='https://img.shields.io/badge/Atividades_Práticas Integradoras (UFMG)-100000?style=plastic&logo=Google Scholar&logoColor=white&labelColor=2F00B0&color=2F00B0'/></a>

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
