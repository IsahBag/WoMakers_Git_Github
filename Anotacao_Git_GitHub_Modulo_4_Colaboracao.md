## Git e GitHub
### Módulo 4: Colaboração

#### Realizando um fork:
  
*No GitHub:*

    1. abrir o repositório que deseja forkear
    2. clicar em 'fork'
    3. vai aparecer uma cópia em seus repositórios

*No git Bash:*

    git clone [https-do-repositorio-forkeado] # irá clonar o repositório para sua máquina
    code .

*No VSCode:*

    git checkout -b add-reame          *cria nova branch
    git push

#### Mantendo o projeto atualizado com o principal:

*Pelo GitHub:*

    ir em 'compare'      # compara os repositório base com o head
    clicar em switch the base caso necessário
    criar uma pull request
    merge pull request
    confirm merge

*Pelo VSCode:*

    git remote add upstream https-do-repositório-forkeado
    git fetch upstream           # tipo um pull
    git rebase upstream/master        # faz o rebalanceamento do que tem na upstream com a master

#### Criando branch para enviar as alterações:

*No VSCode:*

    git checkout -b nome-da-branch
    git commit -m "..."
    git push
    git push --set-upstream origin [nome-da-branch]
    abrir o link da pull request
    open pull request
      - adicionar info no título
      - selecionar revisor
      - assinar
      - no comentário descrever o motivo da pull request

#### Para revisar pull requests:

    1. entrar nas pull request
    2. ir em 'files changed'
    3. no code, clicar no "+" da linha que estou corrigindo
    4. descrever o erro
    5. Start a review
    6. Finish your review
    7. selecionar 'Request changes'
    8. submit review

#### Para alterar os erros apontados: 

*Pelo VSCode:*

    1. realizar as alterações
    2. push

*Avaliar os ajustes do review:*

    1. refazer o processo
    2. Review changes
    3. selecionar approved, se o caso
    4. submit review

*Por fim:*

    1. Merge Pull Request
    2. Confirm Merge
    3. Delete branch