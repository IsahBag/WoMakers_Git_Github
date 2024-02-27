## Git e GitHub
### Módulo 2: Branches

#### Branch:
* separação do código em locais diferentes


*Inicial:*  Branch Master

*Branch Develop:* é disponibilizado  nesse ambiente após testarmos em nossa máquina

*Branch Homolog:* onde as pessoas responsáveis pelo negócio podem validar a solução

*Branch Master:* Branch principal - site que vai ao público

#### Criando uma branch pelo VSCode:

    git checkout -b [nome-da-branch]   # cria uma nova branch e abre a mesma
    git branch                         # lista as branchs existentes
    git checkout [nome-da-branch]      # seleciona a branch que quer abrir
  
#### Criando uma branch pelo GitHub: 

1. Acessar o repositório 
2. Ir na sessão de listagem das branchs 
3. Criar uma nova branch
4. Confirmar a criação dessa nova branch

#### Excluindo uma branch pelo GitHub: 

1. Ir na seção de listagem das branchs 
2. Clique no icone da lixeira

#### Atualizando a branch local com a criada no repositório remoto:

    git push
    git push --set-upstrem origin nome-da-branch
  
#### Comando git merge:                 *faz o merge local
    git checkout master         # volta para a branch principal
    git pull          # atualiza com as modificações feitas no repositório remoto
    git merge [nome-da-branch]     # junta a branch com a master
    git status
    git push    # manda para o repositório remoto