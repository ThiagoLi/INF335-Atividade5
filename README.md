# INF335-Atividade5

# 1 Objetivos
Este trabalho tem como objetivo desenvolver habilidades de uso da ferramenta Jenkins
para integração contínua. Este trabalho compõe a avaliação da disciplina INF335, e
poderá ser realizado individualmente ou em dupla.

# 2 Atividades
Atividade 5.1 – Pipeline Jenkinsfile
Os seguintes passos devem ser realizados:
### 1. Criar projeto no GitHub com resultados do Trabalho 4 (isto é: código fonte,
código de testes, pom.xml).
### 2. Criar arquivo Jenkinsfile com Pipeline no GitHub (incluindo compilação e teste
JUnit).
### 3. Criar item/projeto do tipo Pipeline no servidor Jenkins que acessa e executa o
Jenkinsfile no GitHub.
### 4. Executar Build no Jenkins (verificar no console se todos os passos foram
realizados corretamente, incluindo build e todos os testes bem sucedidos).

# Atividade 5.2 – Jenkins + Docker
Os seguintes passos devem ser realizados:
### 1. Criar projeto no GitHub com a classe Java “OlaUnicamp.java”, com método main
que imprime “Olá Unicamp” no console.
### 2. Criar arquivo Dockerfile no GitHub, que utiliza imagem com jdk (ex:
openjdk:11), copia o arquivo java, executa o compilador (javac) e especifica
execução do comando: java OlaUnicamp.
### 3. Criar arquivo Jenkinsfile com Pipeline para build e execução utilizando Docker.
### 4. Criar item/projeto do tipo Pipeline no servidor Jenkins que acessa e executa o
Jenkinsfile no GitHub.
### 5. Executar Build no Jenkins (verificar no console se a execução ocorreu
corretamente)

# 3 Entrega
Os seguintes itens devem ser entregues:
### 1. Atividade 5.1: Link para repositório (público) com artefatos ne
(incluindo: pom.xml e Jenkinsfile).
### 2. Atividade 5.1: Print com as configurações do projeto no Jenkins.
### 3. Atividade 5.1: Log do console de execução bem sucedida do projeto,
acesso ao repositório Git, compilação, teste e empacotamento (criar .jar
### 4. Atividade 5.2: Link para repositório (público) com artefatos necessários
### 5. Atividade 5.2: Print com as configurações do projeto no Jenkins.
### 6. Atividade 5.2: Log do console de execução bem sucedida do projeto,
acesso ao repositório Git, build do Docker e execução do Docker.
Deverá ser entregue um arquivo por dupla, constando os respectivos nomes e nú
matrículas. As entregas deverão ser realizadas pelo Moodle.

# DATA FINAL DE ENTREGA: 12/05/2023




Started by user INF335
Running as SYSTEM
[EnvInject] - Loading node environment variables.
Building in workspace /var/lib/jenkins/workspace/Freestyle_IC
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --resolve-git-dir /var/lib/jenkins/workspace/Freestyle_IC/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/ThiagoLi/INF335-Atividade5 # timeout=10
Fetching upstream changes from https://github.com/ThiagoLi/INF335-Atividade5
 > git --version # timeout=10
 > git --version # 'git version 2.32.0'
 > git fetch --tags --force --progress -- https://github.com/ThiagoLi/INF335-Atividade5 +refs/heads/*:refs/remotes/origin/* # timeout=10
Seen branch in repository origin/main
Seen 1 remote branch
 > git show-ref --tags -d # timeout=10
Checking out Revision d0ffe3ec000d695906094b8c797521550e769632 (origin/main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f d0ffe3ec000d695906094b8c797521550e769632 # timeout=10
Commit message: "Update README.md"
 > git rev-list --no-walk d0ffe3ec000d695906094b8c797521550e769632 # timeout=10
[Freestyle_IC] $ /bin/sh -xe /tmp/jenkins10707915384889604663.sh
+ cd CODIGO_INF335_Atividade4_Thiago
+ mvn -Dmaven.test.failure=true clean package
[[1;34mINFO[m] Scanning for projects...
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m------------------< [0;36mbr.unicamp.ic.inf335.app:meu-app[0;1m >------------------[m
[[1;34mINFO[m] [1mBuilding meu-app 1.0-SNAPSHOT[m
[[1;34mINFO[m] [1m--------------------------------[ jar ]---------------------------------[m
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m--- [0;32mmaven-clean-plugin:3.1.0:clean[m [1m(default-clean)[m @ [36mmeu-app[0;1m ---[m
[[1;34mINFO[m] Deleting /var/lib/jenkins/workspace/Freestyle_IC/CODIGO_INF335_Atividade4_Thiago/target
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m--- [0;32mmaven-resources-plugin:3.0.2:resources[m [1m(default-resources)[m @ [36mmeu-app[0;1m ---[m
[[1;34mINFO[m] Using 'UTF-8' encoding to copy filtered resources.
[[1;34mINFO[m] skip non existing resourceDirectory /var/lib/jenkins/workspace/Freestyle_IC/CODIGO_INF335_Atividade4_Thiago/src/main/resources
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m--- [0;32mmaven-compiler-plugin:3.8.0:compile[m [1m(default-compile)[m @ [36mmeu-app[0;1m ---[m
[[1;34mINFO[m] No sources to compile
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m--- [0;32mmaven-resources-plugin:3.0.2:testResources[m [1m(default-testResources)[m @ [36mmeu-app[0;1m ---[m
[[1;34mINFO[m] Using 'UTF-8' encoding to copy filtered resources.
[[1;34mINFO[m] skip non existing resourceDirectory /var/lib/jenkins/workspace/Freestyle_IC/CODIGO_INF335_Atividade4_Thiago/src/test/resources
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m--- [0;32mmaven-compiler-plugin:3.8.0:testCompile[m [1m(default-testCompile)[m @ [36mmeu-app[0;1m ---[m
[[1;34mINFO[m] No sources to compile
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m--- [0;32mmaven-surefire-plugin:2.22.1:test[m [1m(default-test)[m @ [36mmeu-app[0;1m ---[m
[[1;34mINFO[m] No tests to run.
[[1;34mINFO[m] 
[[1;34mINFO[m] [1m--- [0;32mmaven-jar-plugin:3.0.2:jar[m [1m(default-jar)[m @ [36mmeu-app[0;1m ---[m
[[1;33mWARNING[m] JAR will be empty - no content was marked for inclusion!
[[1;34mINFO[m] Building jar: /var/lib/jenkins/workspace/Freestyle_IC/CODIGO_INF335_Atividade4_Thiago/target/meu-app-1.0-SNAPSHOT.jar
[[1;34mINFO[m] [1m------------------------------------------------------------------------[m
[[1;34mINFO[m] [1;32mBUILD SUCCESS[m
[[1;34mINFO[m] [1m------------------------------------------------------------------------[m
[[1;34mINFO[m] Total time:  0.696 s
[[1;34mINFO[m] Finished at: 2023-05-12T14:38:16-04:00
[[1;34mINFO[m] [1m------------------------------------------------------------------------[m
Finished: SUCCESS
