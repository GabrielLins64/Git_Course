Curso Git e GitHub Udemy

Comandos Git Básicos:

~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X
Status de arquivos no GIT:

O arquivo pode estar:
 ___________ ____________ __________ ________
| Untracked | Unmodified | Modified | Staged |
|   (ADD)---+------------+----------+--->    |
|           |   (EDIT)---+---->     |        |
|           |            | (STAGE)--+--->    |
|      <----+--(REMOVE)  |          |        |
|           |      <-----+----------+(COMMIT)|
|___________|____________|__________|________|

~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X
Configurações:

git config --global user.name "Nome do usuário"
git config --global user.email "E-mail do usuário"
git config --global core.editor vim # Pra setar o vim como editor padrão
git config user.name # Pro git informar qual o nome do user
git config --list # Mostra todas as informações de config

~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X
Manipulação de Repositório:

git init # Inicia um respositório na pasta atual
git status # informa o status do repositório atual
	Untracked: O arquivo existe mas ainda não foi incluído no git
git add file.etc # Adiciona ao repositório o arquivo "file.etc"
git commit # Dá o commit nos arquivos já adicionados.
git commit -m "Adicione um comentário aqui" # É uma boa prática informar o que foi feito em cada commit
git commit -am "Comentário" # commita todos os arquivos modificados
git commit -om "Comentário" Arquivo # commita apenas o arquivo "Arquivo"
git checkout file # Desfaz as alterações no arquivo modified file
git reset HEAD file # Tira da fila de stageds o arquivo file
git reset --soft hash # Deixa o arquivo commitado como modified staged, na versão da hash informada (não elimina as versões posteriores).
git reset --mixed hash # Volta o arquivo commitado para modified unstaged, na versão da hash informada (não elimina versões posteriores).
git reset --hard hash # Deixa o arquivo commitado (unmodified) mas volta a versão para a da hash informada (ELIMINA VERSÕES POSTERIORES).

~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X
Informações:

git log # Dá informações de log (commits, branches, etc.)
git log --author="Nome do autor" # Procura os Logs apenas do autor informado
git shortlog # Mostra sumariamente informações básicas de logs
git shortlog -sn # Mostra a qtd de commits de cada autor
git log --graph # Mostra, em forma gráfica, os branches e versões.
git show hash # Mostra os detalhes do commit com a hash (informada no log)
git diff # Mostra as modificações feitas nos arquivos.
git diff --name-online # Mostra apenas o nome dos arquivos modificados.

~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X ~~~~~~~~~~~~~~~~~ X
Repositórios remotos (GitHub):

-> Gerando uma chave SSH:

1. Acesse:
	https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh
2. Clique em "Generating a new SSH key"
3. Siga as instruções e gere a chave SSH.
4. Navege em: $cd ~/.ssh/
5. Visualize sua chave pública com: $cat id_rsa.pub
6. Copie a chave (com e-mail e tudo)
7. Adicione ao GitHub em: 
	Settings > SSH and GPG keys > New SSH key
	*É uma boa prática colocar o nome da máquina no title
8. Clique em adicionar SSH.

-> Ligando repositório local a um remoto:

1. Crie um repositório no GitHub (ou abra um existente).
2. 







