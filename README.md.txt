Permite que versoes comitadas possam ser revertidas para o estado Unmodified
	git reset --hard [COMMIT_HASH]
Permite que versoes ja comitadas possam ser vertidas para o estado Modified
	git reset --mixed [COMMIT_HASH]
Permite que versoes ja comitadas possam ser revertidas para o estado Staged
	git reset --soft [COMMIT_HASH]
Permite remover arquivos do estado Staged (git add), devolvendo aos arquivos o estado de modified
	git reset HEAD [NOME_DO_ARQUIVO]
Serve para reverter uma alteração antes de adicionarmos (git add) para commit
	git checkout [NOME_DO_ARQUIVO]
Mostra a diferencia entre o que foi modificado e o que tem para ser comitado
	git diff
	git diff --name-only
Mostra os detalhes de um determinado commit passando como parametro o hash
	git show [COMMIT_HASH]
Commit de um arquivo(s) (on staged)	
	git commit -m"[COMMENT]"
Adicao de um arquivo(s) para commit (ex.: on modified ---> to staged)
	git add [FILENAME]
Exibicao do status geral dos arquivos do controle de versao (untracked, unmodified, modified, staged)
	git status
Exibicao de logs
	git log
	git log --author="[USERNAME]"
	git shortlog
	git shortlog -sn
	git log --graph

SSH
…or create a new repository on the command line
echo "# gitbubcourse" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:souzagonzaga/gitbubcourse.git
git push -u origin master

…or push an existing repository from the command line
git remote add origin git@github.com:souzagonzaga/gitbubcourse.git
git push -u origin master

HTTPS
…or create a new repository on the command line
echo "# gitbubcourse" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/souzagonzaga/gitbubcourse.git
git push -u origin master

…or push an existing repository from the command line
git remote add origin https://github.com/souzagonzaga/gitbubcourse.git
git push -u origin master