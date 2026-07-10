==========================================================================================================
                                          Meu guia de git e GitHub
==========================================================================================================

Índice

1. Bash
2. Git
3. Conceitos
4. Nomes do GitHub 
5. Git Flow
6. Fluxos
7. Estrutura de Projetos
8. Arquivos Especiais
9. Convenções
10. Erros Comuns
11. Analogias
12. Cheat Sheet
13. Perguntas e Respostas 

==========================================================================================================
1.                                                Bash
==========================================================================================================

---Navegação ---

* pwd -> mostra em que pasta eu estou
* ls -> mostra os arquivos da pasta
* ls -a -> mostra os arquivos da pasta e os ocultos também
* cd nome da pasta -> para entrar em uma pasta
* cd .. -> pula uma pasta para cima de onde estou

---Arquivos e Pastas---

* mkdir -> criar uma pasta
* touch -> criar um arquivo tipo README.md
* rm -> apaga ****cuidado
* rm -rf apaga todas as pastas do git pasta e subpasta ****cuidado pode apagar todos os arquivos do Windows
* nano -> editor de texto do terminal integrado nele

==========================================================================================================
2.                                               Comandos Git
==========================================================================================================

--- Iniciar um projeto ---

* git init . -> para inicar um repositorio git e começar o versionamento criação do arquivo .git
Quando usar ? sempre no inicio do projeto
Exem: git init .

--- Configuração ---

* git config --global user.name -> congifurar um user name
Quando usar? na primeira vez para definir um user name 
Exem: git config --global user.name bruna

* git config --global user.email -> configurar um email
Quando usar? na primeira vez para definir um email
Exem: git config --global user.email bruna@gmail.com

--- Estado do projeto ---

* git status -> mostra status atual do projeto, arquivos novos, arquivos modificados, arquivos no staging e branch atual
Quando usar ? sempre que quiser ver o que mudou
Exem: git status

--- Adicionar arquivos ---

* git add . -> adicionar todos os arquivo para o pré-commit stating
Quando usar? antes de fazer commit
Exem: git add .

* git add arquivo -> adicionar apenas 1 arquivo especifico
Quando usar? sempre que não quiser adicionar todos os arquivos
Exem: git add README.md

--- Commit ---
* git commit -m "" -> fazer commit (criado save de uma jogo)
Quando usar ? depois do git add .
Exem: git commit -m "docs: adiciona README"

--- Histórico ---

* git log -> mostra todos os commits bem detalhados
Quando usar ? para ver versões anteriores
Exem: git log

* git log --oneline -> mostra os commits em 1 linha
Quando usar ? para visualização rápida
Exem: git log --oneline

* git log --graph --all -> mostra o histórico em forma de gráfico com todas as branches.
Quando usar ? para ver merge e branches
Exem: git log --graph --all

--- Diferenças ---

* git diff -> mostra a diferença do ultimo commit para a mudança mais recente antes do stating
Quando usar ? antes do git add .
Exem: git diff

* git diff --staged -> mostra a diferença entre o que está no staging e o último commit.
Quando usar ? antes do commit
Exem: git diff --staged

--- Remover do staging ---

* git reset -> tira todos os arquivo do pré-commit
Quando usar ? quando adicionar arquivos no pré-commit por engano
Exem: git reser

* git reset arquivo.txt -> tira arquivo especifico do pré-commit
Quando usar ? quando 1 arquivo foi adicionado por engano no pré-commit
Exem: git reset README.md

--- Branches ---

* git branch -> mostar em qual branch estou indicador por *  ***** muito importante *****
Quando usar ? saber em que branch está
Exem: git brach receita

* git checkout nome da branch -> mudar para outra branch
Quando usar ? mudar de branch
Exem: git checkout main

* git checkout -b nome da branch -> criar uma branch e já muda para ela
Quando usar ? para iniciar uma nova tarefa
Exem: git checkout -b develop

* git switch -> muda para outra branch (comando mais moderno que o checkout)
Quando usar ? no lugar do git checkout

* git switch -c nome_branch -> cria uma nova branch e muda para ela
Quando usar ? no lugar do git checkout
Exem: git switch -c develop

--- Merge ---

* git merge -> junta as alterações da branch informada na branch atual **** importante estar na branch que vai receber o merge antes de fazer o merge ****
Quando usar ? terminar uma funcionalidade
Exem: git merge receita

--- Repositório remoto ---

* git remote add origin -> conecta o repositório local ao repositório do GitHub
Quando usar ?
Exem: na primeira vez que enviar projeto do local para o GitHub

* git remote -v -> mostra os repositórios remotos conectados ao projeto
Quando usar ? ver se a conexão de git e GitHub estão certas
Exem: git remote -v

--- Enviar para GitHub ---

* git push -> enviar repositório para o GitHub
Quando usar ? depois de fazer commits
Exem: git push

* git push origin branch -> enviar branch para o GitHub
Quando usar ? na primeira vez que enviar essa branch ou para atualizar
Exem: git push origin branch develop

* git push -u origin main -> enviar main para o GitHub as 2 mains ficam iguais
Quando usar ? primeiro envio da main
Exem: git push -u origin main

* git push -u origin develop -> enviar develop local para a do GitHub
Quando usar ? primeiro envio da develop
Exem: git push -u origin develop

--- Atualizar do GitHub----

* git pull -> pegar os dados do GitHub para o pc local
Quando usar ? antes de começar a trabalhar ou quando outra pessoa alterou o projeto
Exem: git pull

* git pull origin develop -> pegar os dados atualizados da develop do GitHub para o local
Quando usar ? antes de fazer tarefas na branch develop
Exem: git pull origin develop

--- Buscar informações da nuvem ---

* git fetch -> Baixa as informações mais recentes do GitHub sem alterar sua branch atual.
Quando usar ? para ver se tem novas branch ou commits
Exem: git fetch

--- Arquivos versionados ---

* git ls-file -> ver arquivos que estão sendo versionados pelo git
Quando usar ? para ver qual arquivo faz parte do repositório
Exem: git ls-file

* git clone -> faz clone de um repositório do GitHub para o pc 
Quando usar? para fazer uma copia do projeto do GitHub para o pc
Exem: git clone url

==========================================================================================================
3.                                              Conceitos
==========================================================================================================

--- Git ---

sistema de controle de versão
para controlar alterações do projeto permite voltar versões anteriores
como os saves de um jogo

--- GitHub ---

o que é ? site para armazenar repositórios git na nuvem
compartilhar projetos e colaborar com pessoas

--- Repositório local ---
o que é? projeto salvo no pc

--- Repositório remoto ---
o que é? projeto armazenado no GitHub

--- Commit ---
o que é? regitro das mudaças feitas no projeto
analogia: save de um jogo

--- Head ---
o que é? ponteiro que indica qual foi o ultimo commit da branch atual

--- Branch ---

o que é? uma linha de desenvolvimento independente
analogia: uma missão secundaria derivada da historia principal missão derivada da main

--- Main ---
o que é? branch principal do projeto versão estável do projeto

--- develop ---
o que é? branch onde os funções são salvas e testadas antes de ir para a main deixando a main protegida estão em desenvolvimento 

--- Merge ---
o que é? união do histórico de 2 branch misturando as funções

--- Conflito de merge ---
o que é? quando 2 pessoas alteram a mesma linha de um arquivo o git não sabe qual versão é a certa
como resolver? editar o arquivo manualmente, escolher a versão certa tira as marcações depois fazer git add e git commit tem um indicador merging ao lado das pasta do projeto

--- Origin ---
o que é? nome padrão ao repositório remoto conectado ao projeto

--- Staging área (pré-commit)---
o que é? área temporária onde ficam os arquivos preparados para o próximo commit

--- Untracted ---
o que é? arquivo que o git ainda não monitoria

--- Tracked ---
o que é? arquivo que já esta sendo monitorado pelo git

==========================================================================================================
4.                                         Nomes que aparecem no GitHub
==========================================================================================================

--- Fork ---
O que é? criar uma copia de um repositório na sua conta do GitHub uma copia do projeto do de uma pessoa GitHub para o seu

--- Pull Request ---
O que é? pedir para que suas mudanças sejam analisadas e integradas ao projeto

--- Compare e pull Request ---
O que é? fazer a criação de um pull request para comparar 2 branch

--- Merge Pull Request ---
O que é? aceitar e integrar as alterações do pull request

--- Sync Fork ---
O que é? atualizar seu fork com as alterações do repositório original

--- Collaborators ---
O que é? para adicionar uma pessoa para colaborar no projeto 
é só ir em settings e collaborators e adicionar a pessoa

==========================================================================================================
5.                                              Git Flow
==========================================================================================================

O que é? O Git Flow é uma forma organizada de usar as branches do Git em um projeto. Ele define onde desenvolver, onde testar e quando publicar as alterações.

           main

              ▲

              │

       Merge aprovado

              │

          develop

        ▲    ▲    ▲

        │    │    │

    feat/  fix/ docs/

main
↓
Criar develop
↓
Criar uma branch (feat, fix, docs...)
↓
Desenvolver
↓
git add
↓
git commit
↓
git push
↓
Pull Request
↓
Merge na develop
↓
Testes
↓
Merge na main

main → versão estável do projeto.
develop → reúne todas as funcionalidades em desenvolvimento.
feat/ → novas funcionalidades.
fix/ → correção de bugs.
docs/ → documentação.
Quando todas as alterações estiverem prontas e testadas, a develop é unida à main.

Feature (feat/) → novas funcionalidades.
Fix (fix/) → correções de bugs.
Docs (docs/) → documentação.
Chore (chore/) → tarefas de manutenção.
Release (release/) → preparação de uma nova versão.
Hotfix (hotfix/) → correções urgentes na versão em produção.

==========================================================================================================
6.                                              Fluxos
==========================================================================================================

*** Fluxo normal do Git e GitHub ***

Criar projeto
↓
git init
↓
Criar/editar arquivos
↓
git status
↓
git add
↓
git commit
↓
git push
↓
GitHub
↓
(outra pessoa altera)
↓
git pull
↓
Continuar trabalhando

Você trabalha no computador (Git Local).
Faz commits para salvar versões.
Usa git push para enviar ao GitHub.
Usa git pull para baixar as alterações feitas no GitHub.


*** Fluxo de trabalho em equipe ***

main
↓
develop
↓
Criar uma branch
↓
Editar arquivos
↓
git add
↓
git commit
↓
git push
↓
Pull Request
↓
Revisão
↓
Merge na develop
↓
Testes
↓
Merge na main

Ninguém desenvolve diretamente na main.
Cada pessoa cria sua própria branch.
Depois abre um Pull Request.
Após aprovação, a branch é unida à develop.
Quando tudo estiver pronto, a develop é unida à main.


*** Fluxo para resolver conflito ***

main
Leite

pessoa a altera:
Margarina

pessoa b altera:
Açúcar

ao fazer o merge:
git merge minha_branch

o git mostra:
<<<<<<< HEAD
Margarina
=======
Açúcar
>>>>>>> minha_branch

git merge
↓
Conflito
↓
Editar o arquivo manualmente
↓
Apagar os marcadores
↓
Salvar o arquivo
↓
git add
↓
git commit
↓
Conflito resolvido

O conflito acontece quando duas branches alteram a mesma linha.
O Git para o merge.
Você escolhe manualmente qual versão ficará.
Depois faz git add e git commit.

==========================================================================================================
7.                                            Estrutura de projetos
==========================================================================================================

src/
docs/
tests/
assets/
data/
README.md

==========================================================================================================
8.                                             Arquivos Especiais
==========================================================================================================

.git -> É uma pasta oculta criada pelo Git quando você executa: git init


.gitignore -> É um arquivo de texto que informa ao Git quais arquivos ou pastas não devem ser versionados.
Para que serve?

Evitar enviar ao GitHub arquivos que não precisam fazer parte do projeto, como:
arquivos temporários;
planilhas;
bancos de dados locais;
apresentações;
arquivos grandes;
arquivos de configuração pessoais.
Quando usar?

Sempre que houver arquivos que não precisam ser compartilhados.
Exemplo
*.csv
*.xlsx
*.xls
*.pptx
*.parquet
data/
.env

.gitkeep -> É um arquivo vazio usado apenas para manter uma pasta vazia dentro do repositório.
Para que serve?
O Git não versiona pastas vazias. Se você quiser que uma pasta apareça no GitHub mesmo sem arquivos, coloque um .gitkeep dentro dela.

README.md -> É o arquivo de documentação principal do projeto.

==========================================================================================================
9.                                              Convenções 
==========================================================================================================

--- Branches ---
feat/
fix/
docs/
test/
refactor/
release/
hotfix/
chore/

--- Commits ---
feat:
fix:
docs:
test:
refactor:
chore:

==========================================================================================================
10.                                              Erros Comuns
==========================================================================================================

src refspec does not match any -> git não encontrou a branch ou ela ainda não tem commits
Quando acontece? escrever o nome da branch errado, ainda não foi criada, não tem commits na branch
Resolver? git branch ou criar uma branch git checkout -b nomebranch

permission denied -> Você não tem permissão para enviar alterações para aquele repositório.
Quando acontece?
Está usando a conta GitHub errada.
O repositório pertence a outra pessoa.
Você não é colaborador.
Problemas com autenticação (HTTP ou SSH).
Resolver? git remote -v

Already up to date -> repositório já esta atualizado
Quando acontece? após dar git pull ou git merge

Merge conflict -> alterações diferentes na mesma linha do arquivo e não sabe qual escolher
Quando acontece -> 2 branches modificam a mesma linha
Como resolver?
Abrir o arquivo.
Escolher a versão correta.
Remover os marcadores:
<<<<<<< HEAD
=======
>>>>>>>
Salvar.
Depois:
git add .
git commit -m "resolve conflito"

Detached HEAD -> O HEAD está apontando para um commit e não para uma branch.
Quando acontece? git checkout 4fa38b2
Como resolver? volte para uma branch

fatal -> "Fatal" significa que ocorreu um erro grave e o Git interrompeu o comando.
fatal: not a git repositor -> Você não está dentro de um repositório Git.
fatal: pathspec did not match any files -> O arquivo informado não existe.

nothing to commit -> Não existe nenhuma alteração para salvar em um novo commit.
Quando acontece? depois de git status
Como resolver? Edite algum arquivo primeiro.

working tree clean -> O projeto está limpo. Todos os arquivos já foram commitados.
Quando aparece? após git status
Como resolver? Nada. Essa é uma boa mensagem.

q -> digite q caso o terminal trave depois de algum comando geralmente quando da git log

==========================================================================================================
11.                                              Analogias 
==========================================================================================================

Commit
↓
Save de um jogo

Branch
↓
Missão secundária

Merge
↓
Juntar histórias

Fork
↓
Copiar um livro de receitas

Clone
↓
Baixar esse livro para casa

GitHub
↓
Nuvem

Push
↓
Enviar

Pull
↓
Receber

==========================================================================================================
12.                                          Consulta rápida
==========================================================================================================
git status
git add .
git commit -m ""
git push
git pull
git fetch
git branch
git checkout
git checkout -b
git merge
git log --oneline
git diff
git reset


