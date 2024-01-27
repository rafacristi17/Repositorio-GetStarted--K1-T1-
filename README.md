GITHUB FOLHA DE DICAS DE GIT
V 1.1.1
Git é um sistema de controle de versão distribuído open source que facilita ações com o GitHub em seu notebook ou
desktop. Esta folha de dicas resume instruções comumente usadas via linha de comando do Git para referência
rápida.
INSTALE O GIT
GitHub fornece clientes desktop que incluem uma interface gráfica
para as ações mais comuns em um repositório e atualiza automatica-
mente para a linha de comando do Git para cenários avançados.
GitHub para Windows
https://windows.github.com
GitHub para Mac
https://mac.github.com
FAÇA MUDANÇAS
Revise edições e crie uma transação de commit
$ git status
Lista todos os arquivos novos ou modificados para serem commitados
$ git diff
Mostra diferenças no arquivo que não foram realizadas
$ git add [arquivo]
Distribuições do Git para Linux e sistemas POSIX são disponíveis no
site oficial do Git SCM. Faz o snapshot de um arquivo na preparação para versionamento
Git para todas plataformas
http://git-scm.com Mostra a diferença entre arquivos selecionados e a suas últimas
versões
$ git diff --staged
$ git reset [arquivo]
CONFIGURE A FERRAMENTA
Configure informações de usuário para todos os repositórios locais
$ git config --global user.name "[nome]"
Deseleciona o arquivo, mas preserva seu conteúdo
$ git commit -m "[mensagem descritiva]"
Grava o snapshot permanentemente do arquivo no histórico de versão
Configura o nome que você quer ligado as suas transações de
commit
$ git config --global user.email "[endereco-de-email]"
Configura o email que você quer ligado as suas transações de commit
MUDANÇAS EM GRUPO
Nomeie uma série de commits e combine os esforços completos
$ git config --global color.ui auto $ git branch
Configura o email que você quer ligado as suas transações de commit Lista todos os branches locais no repositório atual
$ git branch [nome-do-branch]
Cria um novo branch
CRIE REPOSITÓRIOS
Inicie um novo repositório ou obtenha de uma URL existente
$ git checkout [nome-do-branch]
Muda para o branch específico e atualiza o diretório de trabalho
$ git init [nome-do-projeto] $ git merge [branch]
Cria um novo repositório local com um nome específico Combina o histórico do branch específico com o branch atual
$ git clone [url] $ git branch -d [nome-do-branch]
Baixa um projeto e seu histórico de versão inteiro Exclui o branch específicoGITHUB FOLHA DE DICAS DE GIT
REFATORE NOMES DOS ARQUIVOS
Mude e remova os arquivos versionados
REVISE HISTÓRICO
Navegue e inspecione a evolução dos arquivos do projeto
$ git rm [arquivo] $ git log
Remove o arquivo do diretório de trabalho e o seleciona para remoção Lista o histórico de versões para o branch atual
$ git rm --cached [arquivo] $ git log --follow [arquivo]
Remove o arquivo do controle de versão mas preserva o arquivo
localmente Lista o histórico de versões para um arquivo, incluindo mudanças de
nome
$ git mv [arquivo-original] [arquivo-renomeado] $ git diff [primerio-branch]...[segundo-branch]
Muda o nome do arquivo e o seleciona para o commit Mostra a diferença de conteúdo entre dois branches
$ git show [commit]
SUPRIMA O RASTREAMENTO
Retorna mudanças de metadata e conteúdo para o commit especificado
Exclua arquivos e diretórios temporários
*.log
build/
temp-*
Um arquivo de texto chamado `.gitignore` suprime o versionamento
acidental de arquivos e diretórios correspondentes aos padrões
específicados
$ git ls-files --other --ignored --exclude-standard
Lista todos os arquivos ignorados neste projeto
SALVE FRAGMENTOS
Arquive e restaure mudanças incompletas
DESFAÇA COMMITS
Apague enganos e crie um histórico substituto
$ git reset [commit]
Desfaz todos os commits depois de `[commit]`, preservando
mudanças locais
$ git reset --hard [commit]
Descarta todo histórico e mudanças para o commit especificado
SINCRONIZE MUDANÇAS
Registre um marcador de repositório e troque o histórico de versão
$ git stash $ git fetch [marcador]
Armazena temporariamente todos os arquivos rastreados modificados Baixe todo o histórico de um marcador de repositório
$ git stash pop $ git merge [marcador]/[branch]
Restaura os arquivos recentes em stash Combina o marcador do branch no branch local
$ git stash list $ git push [alias] [branch]
Lista todos os conjuntos de alterações em stash Envia todos os commits do branch local para o GitHub
$ git stash drop $ git pull
Descarta os conjuntos de alterações mais recentes em stash Baixa o histórico e incorpora as mudanças
Aprenda mais sobre o uso do GitHub e do Git. Envie um email para a
Equipe de Treinamentos ou visite nosso site para ver a agenda de eventos
ou a disponibilidade de cursos particulares.
training@github.com
training.github.com
