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



\--- Configuração ---

* git config --global user.name -> congifurar um user name
* git config --global user.email -> configurar um email



\--- Estado do projeto ---

* git status -> mostra status 
* arquivos novos
* arquivos modificados
* arquivos no staging
* branch atual



\--- Adicionar arquivos ---

* git add . -> adicionar todos os arquivo para o pré-commit stating
* git add arquivo -> adicionar apenas 1 arquivo especifico



\--- Commit ---

* git commit -m "" -> fazer commit (criado save de uma jogo)



\--- Histórico ---

* git log -> mostra todos os commits bem detalhados
* git log -> mostra os commits em 1 linha
* git log --graph --all -> mostra o histórico em forma de gráfico com todas as branches.



\--- Diferenças ---

* git diff -> mostra a diferença do ultimo commit para a mudança mais recente antes do stating

git diff --staged -> mostra a diferença entre o que está no staging e o último commit.



\--- Remover do staging ---

* git reset -> tira todos os arquivo do pré-commit
* git reset arquivo.txt -> tira arquivo especifico do pré-commit



\--- Branches ---

* git branch -> mostar em qual branch estou indicador por \*  \*\*\*\*\* muito importante \*\*\*\*\*
* git checkout nome da branch -> mudar para outra branch
* git checkout -b nome da branch -> criar uma branch e já muda para ela
* git switch -> muda para outra branch (comando mais moderno que o checkout)
* git switch -c nome\_branch -> cria uma nova branch e muda para ela



\--- Merge ---

* git merge -> junta as alterações da branch informada na branch atual \*\*\*\* importante estar na branch que vai receber o merge antes de fazer o merge \*\*\*\*



\--- Repositório remoto ---

* git remote add origin -> conecta o repositório local ao repositório do GitHub
* git remote -v -> mostra os repositórios remotos conectados ao projeto











