# 20 comandos do Git

### 1- git init

É o comando para criar um novo projeto de Git, O comando irá criar um repositório novo em branco.

Exemplo:

**$ git init**

Se você já possui um repositório anterior ou deseja criar um repositório com um nome em específico, você pode passar o nome como parâmetro do comando:

**$ git init <O nome do seu repositório>**



### 2- git add

Esse comando Git adiciona os arquivos especificados de código ao seu repositório, sejam arquivos novos ou arquivos anteriores que foram alterados. Oferece diferentes possibilidades de sintaxe.

Exemplo:

**$ git add seu_arquivo** (esse comando irá adicionar o arquivo em específico ao repositório)

**$ git add \*** (esse comando irá adicionar todos os arquivos novos e/ou modificados ao repositório)



### 3- git config

Quando você está utilizando o Git pela primeira vez ou com uma instalação nova, em um projeto colaborativo, esse comando é fundamental para configurar sua identidade de usuário, inserindo informações como nome e email que serão empregadas em cada *commit*.

Exemplo:

**$ git config –global user.name “Seu nome”**

**$ git config –global user.email “Seu email”**



### 4- git clone

Esse comando Git cria uma cópia exata de um repositório já existente. Ou seja, podemos baixar na nossa máquina o [código fonte](https://blog.betrybe.com/tecnologia/codigo-fonte/) de um repositório remoto.

Exemplo:

**git clone <URL do seu projeto>**



### 5- git commit

É fundamental se estabelecer uma diferença entre git add e git commit:

- git add adiciona seus arquivos modificados à fila para serem submetidos a um commit posteriormente. Os arquivos **não** passaram por um commit.
- O git commit executa o commit dos arquivos que foram adicionados e cria uma nova revisão com um log. Por outro lado, se você não adicionar nenhum arquivo, o git não fará o commit de nada.

É possível combinar as duas ações em um único comando: **$ git commit -a**.

Também é possível adicionar uma mensagem para a execução de um commit. Exemplo:

**$ git commit -m “seu comentário”**



### 6- git branch

É comum na maior parte do tempo possuir múltiplas variações em seu repositório Git, chamadas de *branches* (“ramificações”). A grosso modo, um *branch* é um caminho independente de desenvolvimento, uma alternativa.

A princípio pode parecer fácil se perder em diversos caminhos, mas o comando git branch facilita o gerenciamento de tudo isso. Com diferentes parâmetros, é possível listar, criar ou apagar os *branches**.*

Exemplos:

**$ git branch** (lista todas as ramificações)

**$ git branch <nome_do_branch>** (cria um *branch* com o nome especificado)

**$ git branch -d <nome_do_branch>** (deleta o *branch* com o nome especificado)



### 7- git checkout

Ainda sobre *branches*, esse comando Git pode ser utilizado para trocar de uma ramificação para outra.

Exemplo:

**$ git checkout <nome_do_branch>**

Também é possível combinar operações, criando e fazendo o checkout de um novo *branch* com um único comando:

**$ git checkout -b <nome_do_branch_novo>**



### 8- git pull

O comando Git pull baixa o conteúdo (não os metadados) do que foi alterado no repositório remoto para o seu repositório local e imediatamente atualiza seu contreúdo para a última versão.

Exemplo:

**$ git pull <URL>**



### 9- git rm

Para remover arquivos da sua pasta, você pode utilizar o comando Git rm.

Exemplo:

**$ git rm <nome_do_arquivo>**



### 10- git status

O comando **git status** é usado para verificar as informações sobre o estado atual da nossa branch – que significa “ramo” e corresponde à estrutura do projeto. **Quando criamos um projeto, é criado uma branch chamada master.**

Ao utilizar o comando git status, ele nos mostra as alterações do próximo commit, atualizações que não foram adicionadas, arquivos que não estão sob o controle de versão, entre outras informações pertinentes. 

Exemplo:

**$ git status**

