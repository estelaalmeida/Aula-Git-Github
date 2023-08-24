# **DIO | Resumo Git e GitHub**

Repositório para armazenar resumos sobre Git e GitHub, do Bootcamp Santander 2023.

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

### **Primeiros comandos com o Git**

- Para criar um diretório: `mkdir nome da pasta` ;

- para acessar a pasta: `cd nome-da-pasat/ tabe para completar`;

- para limpara o terminal: `ctrl l` ;

- para transformar em um diretório git: `git: -g init`;

- `git clone pasta a ser clonada`;

- para alterar o nome das pasta: `git clone pasta a ser clonada mesmo comando e passa o novo nome`;

- `git status`;

- Adicionar novos conteúdos ao projeto: `git add.` ;

- Criar um commit: `git commit -m`;

- fleg: `ls -a` ---> lista de arquivos ocultos

- `cat config`: para verificar conteúdo;

- `git remote -v`;

- `cd..` para voltar uma pasta;

- para conectar com dispositivo remoto: git remote add origin link do repossitório;

- para clonar uma Branche especifica : `git clone url —branch nome da branche —single-branch`;

- para criar um arquivo vazio: toch [README.md](http://readme.md/);

- para inserir código `git init`

- para mandar um projeto  `git add origin passata go github`

- para mandar um projeto  `git remote set-url passata go github`

- para mandar um projeto  `git remote set-url origin https:  set-url passar do github`

- para mandar um projeto  `git push origin master`

- para mandar um projeto  `git pull origin master`

- para verificar para onde o commit está apontando `` git log``

- criando ponteiro ``echo "commit-1-branch-main"`> commit-1-branch-main.text

  (``git add .``  + ``git commit -m "nome no commit"``)para criar a branch teste: `` git checkout -b teste`` troca da branch que tá para nova

  para voltar na branch main ``git checkout -b main``

  para lista  os últimos commits branch : ``git branch  -v``

  para que os commts da branch  teste apareça na branch main, precisa ser mesclada:   ` git marge teste` (branch  que vai ser mesclada com o main)

  não vamos mais utilizar a branch teste precisa exclui-lá -> ``git branch ``para listas -->

  para excluir ``git branch  -d teste`` --> para enviar para repositorio ou conectando com o local.

  

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