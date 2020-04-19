Curso Git e GitHub Udemy

Comandos Git Básicos:

git config --global user.name "Nome do usuário"
git config --global user.email "E-mail do usuário"
git config --global core.editor vim # Pra setar o vim como editor padrão
git config user.name # Pro git informar qual o nome do user
git config --list # Mostra todas as informações de config
git init # Inicia um respositório na pasta atual
git status # informa o status do repositório atual
	Untracked: O arquivo existe mas ainda não foi incluído no git
git add file.etc # Adiciona ao repositório o arquivo "file.etc"
git commit # Dá o commit nos arquivos já adicionados.
git commit -m "Adicione um comentário aqui"
	# É uma boa prática informar o que foi feito em cada commit
git log
