#Anotações Git e Github:

###Comandos de apoio:
	Windows:
		Listar diretórios -> dir;
		Mudar diretório -> cd;
		Voltar diretório -> cd .. ;
		Limpar tela -> cls;
		Criar pasta -> mkdir;
		Deletar arquivos em uma pasta -> del;
		Remover pasta -> rmdir;
	Linux:
		Listar diretórios -> ls;
Mudar diretório -> cd;
Voltar diretório -> cd .. ;
Limpar tela -> clear (CTRL+L);
Criar pasta -> mkdir;
Remover pasta -> rm -rf (remove tudo de forma recursiva);

###Como funciona o git por debaixo dos panos:
SHA1 -> É um conjunto de funções hash criptográficas.
Objetos fundamentais -> Blobs, Trees and Commits.
Sistema distribuído;
Segurança.

###Configurando a chave SSH:

No git bash, rode os seguintes comandos:

Gera a chave: ssh-keygen -t ed25519 -C email@gmail.com
Muda para o seguinte diretório: cd /c/Users/NomeUsuário/.ssh/
Abre o arquivo da chave público gerado:  cat id_ed25519.pub

Copia e cola a chave no github no seguinte passo a passo:

Settings -> SSH and GPG keys -> New SSH key -> Ponha um título para identificar qual máquina está configurando e no campo “Key” cole a chave.

Inicie o agente: eval $(ssh-agent -s)

###Primeiros comandos Git:

git init -> inicia um repo git;
git config –global user.email “email@gmail.com” -> configura uma conta do git de forma global;

git config –global user.name NomeUsuário -> configura a conta pelo nome de usuário de maneira global;

git add * -> Adiciona tudo que está na pasta para possível commit;

git commit -m “Nome do commit” -> Realiza o commit ;

git config –list -> Lista as configurações do git na máquina local;

git remote add origin “link do repositório” -> Seta os arquivos locais para um repositório na nuvem (github);

git push origin master -> Sobe para o github os arquivos que estão na “origin” para a branch “master”;

git status -> Verifica o status dos arquivos na máquina local;


