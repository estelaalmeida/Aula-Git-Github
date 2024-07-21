# **DIO |  Git e GitHub**

Repositório para armazenar resumos sobre Git e GitHub
Aprendendo a vercionar códigos  com Git e  GitHub.[Digital Innovation One (https://web.dio.me/c)]

## **📕Documentação**

- [https://git-scm.com/docs/git/pt_BR]
- [https://docs.github.com/pt/get-started]

**dir ->** lista diretórios no Windows no Linux usa-se ls.

**cd/ ->** navegue entre as pastas no Windows e Linux.

**p cd..** -> para voltar um nível na navegação.

**cls ->** para limpar a tela no Windows no Linux clear atalho ctrl +l.

**mkdir -->** cria uma pasta windwos e linux.

**echo hello** tras de volta o que foi passado > redirecionade fluxo.

**del workspace :** deleta apenas arquivos.

**seta para cima :** litar históricos de comando que usei no terminal.

**rmdir workspace /S /Q** :para deletar todo o diretório.

## ***COMO O GIT FUNCIONA***

**SHA1:***_EX. eco "OLÁ MUNDO" | openssl sha1 nome no arquivo*

CRIPTOGRÁFIA;

## **OBJETOS FUNDAMENTAIS DO GIT**

- BLOBS: (armazena o sha) echo 'conteúdo' | git hash-object --stdin(devolve o ha do objeto);
- Sem usar o git echo -e 'blob \conteúdo' | openssl sha1;
- TREES: tree: armazenam blobs , contém metadados, nome do arquivo, mota a estrutura de onde estão os arquivos e outras árvores(contém sha1);
- COMMIT: aponta para o conteúdo todo. contém um sha1;

## **CHAVE SSH E TOKEN**

Contém uma chave pública e outra privada

1. No ícone com a sua foto no git **> Settings** ;
2. **Chaves SSH e gpg;**
3. **Chave SSH --->** Novas chaves SSh : Título e kay;
4. **Git bash --->** ssh-keygen -t ed25519 -c e-mail utilizado no Git;
5. colocar uma senha;
6. **cd/ -->** caminho onde foi mostandra pelo gerenciador ;
7. **SSH** para listar os comandos;
8. **SSH id_ed25519.pub:** motra a chave publica;
9. **copia a chave** e cola na tela do Git no campo : SSH de um título para melhor localização. vai pedir a senha do git novament e pronto.
10. **pwd -->** lista o caminho completo;
11. **inicializar o ssh** : eval$(ssh-agent -s) = gent pid 1382 ;
12. ls para listar --> ssh-add id_ed25519 --> senha;

## **INICIANDO O GIT E CRIANDO UM COMMIT**

### **Comandos Git**

- Adiciona um repositório remoto com um nome específico:
        ``git remote add [nome-remoto] [URL]``

- Utiliza para  efetuar push das alterações  locais para o repositório online:
        ``git pusnh add origin main``

- Para recuperar as útimas alterações  do repositórios remoto,mas não faz merge automático:
    	  ``git fetch``
  
- Desfaz as alterações  no arquivo especifico, removendo-o do ídice:
        ``git reset [arquivo]``
  
- Remve um arquivo do repositório e o incluí no próximo commit:
        ``git rm [arquivo]``
  
- Mostra as diferenças entre as alterações que não foram adicionado ao índice:
          ``git diff``

- Para criar um diretório:
          `mkdir nome da pasta`

- Para acessar a pasta:
          `cd nome-da-pasat/ tabe para completar`

- Para limpara o terminal:
          `ctrl l` 

- Para transformar em um diretório git:
          `git: -g init`
  
- Para clonar um repositório:
          `git clone pasta a ser clonada`
  
- Para alterar o nome das pasta:
          `git clone pasta a ser clonada mesmo comando e passa o novo nome`
  
- Para verificar o andamento do projeto no git:
          `git status`

- Adicionar novos conteúdos ao projeto:
          `git add.`

- Criar um commit:
          `git commit -m`

- lista de arquivos ocultos:
          fleg: `ls -a`

-Para verificar conteúdo;
          `cat config` 

-Para voltar uma pasta: 
          `cd..`

- Para conectar com dispositivo remoto:
          ``git remote add origin link do repossitório``

- Para clonar uma Branche especifica:
          `git clone url —branch nome da branche —single-branch`

- Para criar um arquivo vazio:
          ``toch [README.md](http://readme.md/)``

- Para inserir código:
           `git init`

- Para mandar um projeto:
            `git add origin passata go github`

- Para mandar um projeto:
            `git remote set-url passata go github`

- Para mandar um projeto:
            `git remote set-url origin https:  set-url passar do github`

- Para enviar commits do repositório local para o remoto:
            `git push origin master`

- Para atualizar o repositório local com o remoto:
            `git pull origin master`

- Para verificar para onde o commit está apontando e lista-los:
            ``git log``
  
- Para listar todas as branches locais e destaca a branch atual:
            ``git branch``
  
- Para criar uma nova branch(UTILIZADO QUANDO FAZEMOS ALTERAÇÕESSEM AFETAR A BRANCH ORIGINAL:
          ``git branch [nome-da-branch]``
  
- Para alterar para um branch específica:
          ``git checkout [nome-da-branch]``.
  
- Para combinar  as alterções  de uma branch para uma branch atual:
          ``git merge [branch]``
  
- Para listar os repositórios remotos configurados:
          `git remote -v``

- Criando ponteiro:
          ``echo "commit-1-branch-main"`> commit-1-branch-main.text

              (``git add .``  + ``git commit -m "nome no commit"``)para criar a branch teste: `` git checkout -b teste`` troca da branch que tá para nova

- Para voltar na branch main:
          ``git checkout -b main``

- Para lista  os últimos commits branch :
          ``git branch  -v``

  Para que os commts da branch  teste apareça na branch main, precisa ser mesclada:
          `git marge teste` (branch  que vai ser mesclada com o main)

  Não vamos mais utilizar a branch teste precisa exclui-lá:
         ``git branch ``para listas -->

  Para excluir:
          ``git branch  -d teste`` --> para enviar para repositorio ou conectando com o local.
  
  

  ## CONFLITOS DE MERGE

  - ``git log`` para verificar para onde está apontando  volta no git  --> {``git add .`` + ``git commit -m "nome do novo commit" --> git push origin main --> git pull faz a alteração necessária e git add . + novo commit -m "novo commit" + git push(para enviar as auterações para o repositório)``

  - Comando para  baixar alterações do repositório e não vai mesclar `` git fetch origin main``
  - para ver a diferença da branch main com a mater `` git diff main orinrin/main``
  - para trazer as alterações do git remoto para o repositório local depois do comando acima``git marge origin;main``
  - para clona apenas uma branch ``git clone "link do repositório" --branch teste --single-b branch``   para ficar separado``git stash`` ``git stash list``
  - para voltar para outra branch ``git checkout -b  teste-

  2``   git checkout teste``

  - para adicionar novo e excluir o antigo  ``git stash pop`` ou`` git stash apply``  

  

##   **RESOLVENDO CONFLITOS**

- Quando o código está diferente ao que está no GitHub: Será necessário clonar o condigo do Git e modificar para o arquivo correto.
- `Git pull origin master` (para puxar o arquivo alterado no github). conflito de linha. terá que corrigir o conteúdo diferente.
- `git add *` **-->** commit -m na atualização realizada --> `git push origin master`.



###  **BRANCHES**

main -> commit 0 -> commit 1 -> commit 3 - >(teste)









### **Fonte: Aula Git e GitHub da DIO**
