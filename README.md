\# Meu guia de git e GitHub



* Bash



\---Navegação---



* pwd -> mostra em que pasta eu estou
* ls -> mostra os arquivos da pasta
* ls -a -> mostra os arquivos da pasta e os ocultos também
* cd nome da pasta -> para entrar em uma pasta
* cd .. -> pula uma pasta para cima de onde estou



\---Arquivos e Pastas---



* mkdir -> criar uma pasta
* touch -> criar um arquivo tipo README.md
* rm -> apaga \*\*\*\*cuidado
* rm -rf apaga todas as pastas do git pasta e subpasta \*\*\*\*cuidado pode apagar todos os arquivos do windows





* Git





\--- Iniciar um projeto ---

* git init . -> para inicar um repositorio git e começar o versionamento criação do arquivo .git

Quando usar ? sempre no inicio do projeto

Exem: git init .



\--- Configuração ---

* git config --global user.name -> congifurar um user name
* git config --global user.email -> configurar um email



\--- Estado do projeto ---

* git status -> mostra status atual do projeto, arquivos novos, arquivos modificados, arquivos no staging e branch atual

Quando usar ? sempre que quiser ver o que mudou

Exem: git status



\--- Adicionar arquivos ---

* git add . -> adicionar todos os arquivo para o pré-commit stating

Quando usar? antes de fazer commit 

Exem: git add .



* git add arquivo -> adicionar apenas 1 arquivo especifico

Quando usar? sempre que não quiser adicionar todos os arquivos

Exem: git add README.md 



\--- Commit ---

* git commit -m "" -> fazer commit (criado save de uma jogo)

Quando usar ? depois do git add .

Exem: git commit -m "docs: adiciona README"





\--- Histórico ---

* git log -> mostra todos os commits bem detalhados

Quando usar ? para ver versões anteriores 

Exem: git log



* git log --oneline -> mostra os commits em 1 linha

Quando usar ? para visualização rápida 

Exem: git log --oneline



* git log --graph --all -> mostra o histórico em forma de gráfico com todas as branches.

Quando usar ? para ver merge e branches

Exem: git log --graph --all



\--- Diferenças ---

* git diff -> mostra a diferença do ultimo commit para a mudança mais recente antes do stating

Quando usar ? antes do git add .

Exem: git diff



* git diff --staged -> mostra a diferença entre o que está no staging e o último commit.

Quando usar ? antes do commit

Exem: git diff --staged



\--- Remover do staging ---

* git reset -> tira todos os arquivo do pré-commit

Quando usar ? quando adicionar arquivos no pré-commit por engano

Exem: git reser



* git reset arquivo.txt -> tira arquivo especifico do pré-commit

Quando usar ? quando 1 arquivo foi adicionado por engano no pré-commit

Exem: git reset README.md 



\--- Branches ---

* git branch -> mostar em qual branch estou indicador por \*  \*\*\*\*\* muito importante \*\*\*\*\*

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



* git switch -c nome\_branch -> cria uma nova branch e muda para ela

Quando usar ? no lugar do git checkout

Exem: git switch -c develop



\--- Merge ---

* git merge -> junta as alterações da branch informada na branch atual \*\*\*\* importante estar na branch que vai receber o merge antes de fazer o merge \*\*\*\*

Quando usar ? terminar uma funcionalidade

Exem: git merge receita



\--- Repositório remoto ---

* git remote add origin -> conecta o repositório local ao repositório do GitHub

Quando usar ? 

Exem: na primeira vez que enviar projeto do local para o GitHub 



* git remote -v -> mostra os repositórios remotos conectados ao projeto



\--- Enviar para GitHub ---

* git push -> enviar repositório para o GitHub
* git push origin branch -> enviar branch para o GitHub
* git push -u origin main -> enviar main para o GitHub as 2 mains ficam iguais
* git push -u origin develop -> enviar develop local para a do GitHub



\--- Atualizar do GitHub

* git pull -> pegar os dados do GitHub para o pc local
* git pull origin develop -> pegar os dados atualizados da develop do GitHub para o local



\--- Buscar informações da nuvem ---

* git fetch



\--- Arquivos versionados ---

* git ls-file -> ver arquivos que estão sendo versionados pelo git 



* git clone -> faz clone de um repositório do GitHub para o pc usado no fork





\--- Git ---

é fazer um checkpoint do código para vc poder voltar a qualquer parte do código sem perder nada





Fork

Pull Request

Compare e pull Request

Merge Pull Request

Sync Fork

&#x20;

