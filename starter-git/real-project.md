# See changes at different points in the story.
- git show hash-value
# Color only the modifications
- git show hash-value --color-words
# See only specific modifications with show.
- git show hash-value -- src/views/*
# ignoring unwanted files or directories.
- Using vim, create .gitignore and type the name of the file to be ignored.
- git rm -r --cached .(lmpando tudo que tem no cache, basicamente, o git para de rastrear os arquivos)
- git add .
- git commit -m "ignoring files"

# Anotações complementares sobre o .gitignore
Criar o .gitignore com o vim, escrever dentro o nome do arquivo ou pasta a ser ignorado, salva o arquivo, e adiciona no reposiório local. 
