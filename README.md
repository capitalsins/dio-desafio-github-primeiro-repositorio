# Desafio de Projeto sobre Git/Github
Um desafio de projeto de conhecimento de Git e GitHub

<br>

## Diferença entre Git e GitHub:
* Git - Sistema de controle de versão
* GitHub - Plataforma web onde conseguimos colocar projetos que estão versionados usando Git

<br>

## GIT:
* pwd --> Mostra o caminho da pasta atual em que está.
* clear --> Limpa tudo do terminal.
* ls --> Lista todos os arquivos que tem dentro dessa pasta.
* mkdir --> (make a directory) Cria uma pasta, ou um diretório ex: mkdir git_github
* cd --> (change directory) Navegua entre pastas ex: cd git_github
* cd .. --> Volta a página anterior
* rm -d --> (remove directory) Para remover um diretório e não um arquivo.
* rm -r --> O r é de recursivo, remover uma pasta com arquivos dentro.

<br>

## CONFIGURAÇÕES DO GIT COM GITHUB:
- Configuração do teu usuário localmente pra poder trabalhar com o GitHub, só precisa fazer isso uma vez no computador, e as informações vão ficar guardadas, salvas ali pra sempre
- O Git vem com a ferramenta, que é o Git Config, que a gente consegue atribuir váriaveis e fazer algumas outras configurações de usuários na nossa máquina, no nosso computador.
- Essas variáveis, esses arquivos, eles conseguem ser armazenados em 3 lugares.
- 1 Lugar: Seria no nosso computador de forma global, todos os usuários ficariam com a mesma configuração.
- 2 Lugar: Configuração pra usuários específicos.
- 3 Lugar: Configuração pra repositórios, ou projetos específicos.
- Cada nível desse sobrescreve o outro
- Pra conseguir fazer commits, fazer as operações, a gente precisa ter um usuário autenticado na máquina e também um usuário autenticado no GitHub.
- Essa informação vai ficar carimbada nos nossos commits de forma imutável, pra dizer quem que fez esse commit
- git config
    - Configurar o username globalmente:
        - git config —global user.name “Capitalsins”
    - Configurar o email:
        - Caso tenha um email no GitHub já cadastrado, melhor usar do GitHub, ou colocar a tua conta principal.
        - git config —global user.email “seuprincialemail@mail.com”
    - Testar configurações pra ver se está tudo certo:
        - git config —list
        - lista essas configurações
    - Buscar configuração específica no git config:
        - git config user.name, vai mostrar o usuário que cadastrou

<br>

## O que é o GitHub?
* SERVIÇO ONDE PODEMOS CRIAR PROJETOS, DENTRO DE REPOSITÓRIOS, E COMPARTILHAR ISSO COM OUTRAS PESSOAS

<br>

## Comandos GITHUB:

**git init**

* vai ter que fazer pra cada repositório novo que criar, para inicializar o git, ou usando o git clone que já vem com a pasta .git

**git branch -m main**

* trocar o nome do Branch pra main

**git remote add origin [https://github.com/user.name-repository.git](https://github.com/user.name-repository.git)**

* linka nosso repositório local com o repositório remoto, adiciona uma origem, um link de conexão entre o repositório local e o repositório remoto

**git remote -v**

* verifica se está funcionando normalmente

**git status**

* mostra o estado atual dos arquivos na minha pasta

**git add**

* **git add nome-do-arquivo**

* Ex:

    * **git add index.html**

    * vai mandar o arquivo index.html para o status de STAGED, para que possa commitar depois.

**git add .**

* vai mandar todos os arquivos para staged

**git commit**

* **git commit -m "mensagem clara do que está sendo commitado"**

* Ex:

    * **git commit -m "Trocado de camiseta para camisa"**

    * O commit é como se fosse um "ponto de salvamento" no controle de versão do git, tudo que estiver commitado pode ser enviado por push para o repositório remoto.

**git push**

* git push carrega todos os commits da branch local para o branch remoto correspondente.

* Seria o último passo, basicamente faria o push(empurrar), empurraria as modificações que fez localmente pro GitHub

* só precisa fazer esse comando a primeira vez no diretório

* Ex:

    * **git push -u origin main**

**git clone**

* É um comando que serve pra clonar um repositório remoto na minha máquina local, ou seja vou pegar o repositório remoto e transformar ele no repositório local no meu computador

* Serve pra pular alguns comandos, tipo git init, git remote, ele já faz isso.

* Ex:

    * git clone [https://github.com/capitalsins/dio-desafio-github-primeiro-repositorio.git](https://github.com/capitalsins/dio-desafio-github-primeiro-repositorio.git)

**git pull**

* Serve pra puxar as versões mais recentes dos arquivos de um repositório remoto, é muito usado quando trabalho em equipe

* Pra fazer um git pull precisa estar dentro do repositório que a gente quer fazer o pull, que a gente quer puxar as alterações do repositório remoto

* Neste repositório local, faz um git pull e busca daquela url remota, vê se tem alterações arquivos novos, pastas novas, qualquer tipo de alteração que tiver lá, ele vai baixar pra mim

* Ideal colocar o nome do branch que está dando pull

* Usado para buscar e baixar conteúdo de repositórios remotos e fazer a atualização imediata ao repositório local para que os conteúdos sejam iguais.

* Para o git pull funcionar, o diretório o qual está, tem que ter inicializado pelo menos o git. --> git init

* Ex:

    * git init

    * git pull [https://github.com/capitalsins/dio-desafio-github-primeiro-repositorio.git](https://github.com/capitalsins/dio-desafio-github-primeiro-repositorio.git)
