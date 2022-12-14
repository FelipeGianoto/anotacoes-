<h1> Maven: gerenciamento de dependências e build de aplicações Java </h1>


As principais vantagens de se utilizar o Maven em uma aplicação Java
- Gerenciamento de dependências
- Automatização do build

O  mvn --help. Tem vários comandos que podemos utilizar. Temos, por exemplo,  mvn  --projects para listar os projetos,  mvn --settings para atualizarmos as configurações do Maven,  update etc.

As principais maneiras de se utilizar o Maven?
- Pelo prompt de comandos
- Pela integração com a IDE

GroupId
- Para identificar, unicamente, a organização ao qual o projeto pertence

Um dos sources folders presentes em um projeto Maven é o src/main/resources. Que tipos de arquivos normalmente encontramos nesse source folder?
- Arquivos de configuração

Por qual motivo precisaríamos adicionar algum repositório remoto?
- Para baixar dependências que não estão no repositório central do Maven

Vimos que podemos executar o build da aplicação com o comando mvn goal, sendo goal o nome da tarefa que queremos solicitar ao Maven para executar. Qual o objetivo do goal test?
- Executar os testes automatizados da aplicação

Qual o objetivo de se utilizar plugins?
- Adicionar novas funcionalidades ao Maven

Como o Maven identifica os módulos de um projeto?
- Pela tag  <modules> adicionada no pom.xml
