## Git e GitHub
### Módulo 2: Criando repositórios

#### Criando um repositório local:

1. *Git Bash:*

        mkdir [nome-do-repositorio]   # cria um diretório
        ls                            # mostra o conteúdo
        cd [nome-do-repositório]      # abre o diretório
        code .                        # abre o diretório no vs code

2. *Terminal do VS code:*

        git config --list             # lista as configurações
        git init			           # git reconhece como conteúdo rastreável

#### Conectando um repositório local com um remoto:

1. *GitHub:*

        criar um repositório
        após criar, na página que abrir ir em 'quick setup'
        copiar a linha "git remote add origin [https]"

2. *Terminal do VS code*

        git remote -v            # verifica se tem origem remota
        colar no terminal do VS  # cria a origem remota
        git remote -v            # confere a criação da origem remota

#### Clonando um repositório já existente:

1. *Terminal VS Code*

        cd ../                        # volta para a pasta raiz
        mkdir teste-clone             # cria o diretório
        cd teste-clone                # abre a pasta
        copiar o https da página  
        git clone [https]
        ls
        code .                    # abre o diretório em novo arquivo no VS Code

#### Comando git status:             
    git status            # mostra status dos arquivos dentro do repositórios

#### Comando git add:                
    git add .                     # adiciona todos os arquivos da fila da esteira do commit
    git add [caminho do arquivo]  # adiciona o arquivo especificado

#### Comando git commit:  
* registro do status dos arquivos do repositório           
* permite a visualização do histório de todos os commits
* permite a reversão de algum commit

      git commit -m "descrição_da_modificação"

#### Comando git branch:  

    git branch -m main       # cria a branch main

#### Comando git push:     
* atualiza o respositório remoto com as alterações no repositório local

        git push
        git push --set-upstream origin master *gera a origem remota com a branch master

#### Comando git pull:   
* atualiza o repositório local com as alterações no repositório remoto            
  
      git pull