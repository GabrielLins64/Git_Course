Curso Git e GitHub Udemy

Comandos Git Básicos:

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
git commit -m "Adicione um comentário aqui"
	# É uma boa prática informar o que foi feito em cada commit
git commit -am "Comentário" # commita todos os arquivos modificados
git commit -om "Comentário" Arquivo # commita apenas o arquivo "Arquivo"
git checkout file # 

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



