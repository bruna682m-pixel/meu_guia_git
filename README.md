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

Quando usar ? ver se a conexão de git e GitHub estão certas

Exem: git remote -v



\--- Enviar para GitHub ---

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



\--- Atualizar do GitHub

* git pull -> pegar os dados do GitHub para o pc local

Quando usar ? antes de começar a trabalhar ou quando outra pessoa alterou o projeto

Exem: git pull



* git pull origin develop -> pegar os dados atualizados da develop do GitHub para o local

Quando usar ? antes de fazer tarefas na branch develop

Exem: git pull origin develop





\--- Buscar informações da nuvem ---

* git fetch -> Baixa as informações mais recentes do GitHub sem alterar sua branch atual.

Quando usar ? para ver se tem novas branch ou commits

Exem: git fetch



\--- Arquivos versionados ---

* git ls-file -> ver arquivos que estão sendo versionados pelo git

Quando usar ? para ver qual arquivo faz parte do repositório 

Exem: git ls-file



* git clone -> faz clone de um repositório do GitHub para o pc usado no fork





\--- Git ---

sistema de controle de versão

para controlar alterações do projeto permite voltar versões anteriores

como os saves de um jogo



\--- GitHub ---

o que é ? site para armazenar repositórios git na nuvem

compartilhar projetos e colaborar com pessoas



\--- Repositório local ---

o que é? projeto salvo no pc



\--- Repositório remoto ---

o que é? projeto armazenado no GitHub



\--- Commit ---

o que é? regitro das mudaças feitas no projeto

analogia: save de um jogo



\--- Head ---

o que é? ponteiro que indica qual foi o ultimo commit da branch atual



\--- Branch ---

o que é? uma linha de desenvolvimento independente

analogia: uma missão secundaria derivada da historia principal missão derivada da main



\--- Main ---

o que é? branch principal do projeto



\--- develop ---

o que é? branch onde os funções são salvas e testadas antes de ir para a main deixando a main protegida



\--- Merge ---

o que é? união do histórico de 2 branch misturando as funções 



\--- Conflito de merge ---

o que é? quando 2 pessoas alteram a mesma linha de um arquivo o git não sabe qual versão é a certa

como resolver? editar o arquivo manualmente, escolher a versão certa tira as marcações depois fazer git add e git commit tem um indicador merging ao lado das pasta do projeto



\--- Origin ---

o que é? nome padrão ao repositório remoto conectado ao projeto



\--- Staging área (pré-commit)---

o que é? área temporária onde ficam os arquivos preparados para o próximo commit



\--- Untracted ---

o que é? arquivo que o git ainda não monitoria 



\--- Tracked ---

o que é? arquivo que já esta sendo monitorado pelo git







Fork

Pull Request

Compare e pull Request

Merge Pull Request

Sync Fork

&#x20;

