# :bookmark: Desafio projeto Git/Github da DIO

## Repositório 

Projeto sobre Git/Github

## Links úteis :arrow_down:
[Sobre Markdown](https://www.markdownguide.org/getting-started/)

[Sobre Git Bash](https://www.atlassian.com/br/git)



# :boom: Conceitos e comandos do Git :boom:

#### :question: Diferença de Git e Github :cat:

O Git é uma ferramenta de controle de versão local, enquanto o GitHub é uma plataforma online que permite hospedar projetos Git e colaborar com outras pessoas.

#### Oque é o Git :arrow_down:

O Git é um sistema de controle de versão distribuído, o que significa que um clone local do projeto é um repositório de controle de versão completo. 
Esses repositórios locais totalmente funcionais facilitam o trabalho offline ou remotamente.

#### Oque é uma Branch :arrow_down:

Em termos simples, uma branch é literalmente uma ramificação da base do código. 
Enquanto mantemos o código de produção na branch principal (por exemplo), podemos criar uma ramificação para trabalhar livremente neste código e somente depois juntar (mergear) estes códigos.

#### :notebook: Comando Git básicos :arrow_down:  

1. ***git config***

  Quando você está utilizando o Git pela primeira vez ou com uma instalação nova, em um projeto colaborativo, esse comando é fundamental para configurar sua identidade de usuário, inserindo informações como nome e e-mail que serão empregadas em cada commit.

Exemplo:

$ git config –global user.name “Seu nome”

$ git config –global user.email “Seu email”

2. ***git init***

  Esse é o comando que você irá utilizar para criar um novo projeto de Git. O comando irá criar um repositório novo em branco e, a partir daí, será possível armazenar seu código fonte, alterar, salva guardar alterações etc.

Exemplo:

$ git init

Se você já possui um repositório anterior ou deseja criar um repositório com um nome em específico, você pode passar o nome como parâmetro do comando:

$ git init <O nome do seu repositório>

3. ***git clone***

  Esse comando Git cria uma cópia exata de um repositório já existente.

Então… quando usar git init e quando usar git clone? O git clone é mais avançado, uma vez que ele mesmo executa um comando git init internamente. Além disso, ele verifica todo o conteúdo do projeto.

Exemplo:

git clone <URL do seu projeto>

4. ***git add***

Esse comando Git adiciona os arquivos especificados de código ao seu repositório, sejam arquivos novos ou arquivos anteriores que foram alterados. Oferece diferentes possibilidades de sintaxe.

Exemplo:

$ git add seu_arquivo (esse comando irá adicionar o arquivo em específico ao repositório)

$ git add * (esse comando irá adicionar todos os arquivos novos e/ou modificados ao repositório)

5. ***git commit***

  É fundamental se estabelecer uma diferença entre git add e git commit:

git add, adiciona seus arquivos modificados à fila para serem submetidos a um commit posteriormente. Os arquivos não passaram por um commit.
O git commit executa o commit dos arquivos que foram adicionados e cria uma nova revisão com um log. Por outro lado, se você não adicionar nenhum arquivo, o git não fará o commit de nada.
É possível combinar as duas ações em um único comando: $ git commit -a.

Também é possível adicionar uma mensagem para a execução de um commit. Exemplo:

$ git commit -m “seu comentário”

6. ***git branch***

  É comum na maior parte do tempo possuir múltiplas variações em seu repositório Git, chamadas de branches (“ramificações”). A grosso modo, um branch é um caminho independente de desenvolvimento, uma alternativa.

A princípio pode parecer fácil se perder em diversos caminhos, mas o comando git branch facilita o gerenciamento de tudo isso. Com diferentes parâmetros, é possível listar, criar ou apagar os branches.

Exemplos:

$ git branch (lista todas as ramificações)

$ git branch <nome_do_branch> (cria um branch com o nome especificado)

$ git branch -d <nome_do_branch> (deleta o branch com o nome especificado)

7. ***git checkout***
   Ainda sobre branches, esse comando Git pode ser utilizado para trocar de uma ramificação para outra.

Exemplo:

$ git checkout <nome_do_branch>

Também é possível combinar operações, criando e fazendo o checkout de um novo branch com um único comando:

$ git checkout -b <nome_do_branch_novo>

#### :notebook: Comandos Git intermediários :arrow_down:

8. ***git remote***
   O comando Git remote estabelece uma conexão entre seu repositório local e um repositório remoto.

Exemplo:

$ git remote add <nomecurto> <url>

9. ***git push***

Esse comando serve para subir suas modificações para um repositório remoto conectado anteriormente com git remote.

Exemplo:

$ git push -u <nome_curto> <nome_do_branch>

É importante especificar a origem e o upstream antes de usar o git push. Veja o exemplo:

$ git push –set-upstream <nome_curto> <nome_do_branch>

10. ***git fetch***
    Quando você precisa baixar as mudanças criadas por outros membros do seu projeto colaborativo, você precisa do comando Git fetch. A partir desse comando, você irá receber todas as informações de commits, para avaliar, antes de aplicar essas alterações na sua versão local do repositório.

Exemplo:

$ git fetch

11. ***git pull***
    O comando Git pull baixa o conteúdo (não os metadados) do que foi alterado no repositório remoto para o seu repositório local e imediatamente atualiza seu contreúdo para a última versão.

Exemplo:

$ git pull <URL>

14. ***git rm***
    Para remover arquivos da sua pasta, você pode utilizar o comando Git rm.

Exemplo:

$ git rm <nome_do_arquivo>

15. ***git help***
    Existem inúmeros comandos no Git, muito mais do que os 16 dessa lista, cada um com sua função, parâmetros e características. Felizmente, o próprio Git tem o comando help para trazer ajuda diretamente no terminal.

Exemplo:

$ git help <comando que se tem dúvida>

16. ***git merge***

Esse comando Git integra as mudanças de dois branches diferentes em um único branch. Ele precisa ser iniciado a partir de um branch já selecionado, que será mesclado com outro, com o nome passado por parâmetro.

Exemplo:

$ git merge <nome_do_branch>



Abaixo vou deixar sites de referência para auxiliar se tiver alguma dúvida .



:arrow_right: [Git](https://learn.microsoft.com/pt-br/devops/develop/git/what-is-git) 

:arrow_right: [Branchs](https://git-scm.com/book/pt-br/v2/Branches-no-Git-Branches-em-poucas-palavras) 

:arrow_right: [Github](https://www.hostinger.com.br/tutoriais/o-que-github#:~:text=Em%20suma%2C%20o%20GitHub%20%C3%A9,registro%20detalhado%20do%20seu%20progresso)




