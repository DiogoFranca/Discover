# Step 01

O ssh é um tipo de conexão para conectar sua maquina com os servidores do github. Para identificar se a maquina tem autorização pra acessar tal conta.

Intruções: senta ao lado do perfil > settings > ssh and GPG Keys...

Agora, abri o terminal, digite o comando: ssh-keygen -t rsa -f 4096 -C "diogofranca845@gmail.com"

Em seguida, temos que pegar a chave, use o comando: cat ~/.ssh/id_rsa.pub, depois, copie o a chave apartir de "ssh-rsa..."

Adicione o que copiou no SSH and GPG Keys

Abrir no navegador o site: https://docs.github.com/pt/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent, seguia as instruções do site.

Iniciar ssh-agent no terminal: eval "$(ssh-agent -s)"

E digitar esse comando: ssh-add ~/.ssh/id_rsa

# Step 02: linka repositório local com o remoto.

Crie um repositório e adicione uma descrição, não adiciona o readme, vai ser manualmente.

Crie um repositório git com git init, crie o README.md no repo com vim, commita o readme.md.

O próprio github vai informa-lhe os próximos comandos para linkar.

Adicionar repositório remoto: git remote add origin (se usa o ssh é mais seguro) git@github.com:DiogoFranca/teste.git/ git remote -v(ver os links na nuvem)

Crie o branch main: git branch -m main(ainda não temos um branch main)

git push -u(para que local estou enviando na nuvem) origin main(é apenas para liberar o acesso a nuvem, uma única vez)

*Gravatar(foto)

Só precisa de git push para lançar suas alterações.

Pra pegar alterações feitas no github apenas use o git pull.

# Step 03: corrigindo conflitos de merge

git config --global pull.rebase false

pode haver um conflito, abra o arquivo com conflito no vscode, e lá, mostrará opções para se escolher.

Após isso, faça o commit do fixing merge.

E, faça um pull para ver que foi corrigida, e, depois, faça um push.

# Clone

Vai no repositório, em code, ssh e copie.

git clone (ssh)





