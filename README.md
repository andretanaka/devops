<h1>DevOps</h1>
Apresentação sobre Linux

<h2>Atalhos de teclado</h2>

```
tab
ctrl + r
```

<h2>Comandos Linux</h2>

Listar o conteúdo de um diretório

```
ls -la
```

Verificar o diretório que o usuário esta situado.

```
pwd
```

Mudando de diretório

```
cd [diretório]
cd .. - Volta um diretório
cd / -  Volta para a raíz
cd ~ -  Volta para a home do usuário atual
cd - -  Volta para o diretório anterior
```

Ajuda sobre um comando

```
man [comando]
[comando] --help
```

Criar um diretório

```
mkdir [diretorio]
```

Remove um diretório

```
rmdir [diretorio]   
rmdir -r [diretorio]
```
vim texto.txt - abre o arquivo texto.txt no vim
touch texto.txt - cria o arquivo texto.txt
echo "texto" > texto.txt - cria o arquivo texto.txt com o "texto" escrito nele
echo "texto" >> texto.txt - concatena no final do arquivo
cat texto.txt - exibe o conteudo do arquivo texto.txt
> texto.txt - cria o arquivo texto.txt e se ele existir, apaga o conteudo dele
alias ll="ls -la" - cria o alias ll com o comando ls -la
unalias ll - remove o alias ll
ps -ef - exibe os processos em execucao sem infos de processamento e memoria usados
top - exibe os processos em execucao com infos de processamento e memoria usados
kill -9

chmod -R u+rwx g-rwx o+rwx arquivo/diretorio
chmod -R 777 arquivo diretorio

chown novousuario arquivo/diretorio
chown novousuario:novogrupo arquivo/diretorio
chown :novogrupo arquivo/diretorio

Sistema de permissoes
-rwxrwxrwx
primeira letra = Natureza do arquivo:
d	Diretório
l	Link

Proximos 3 grupos de 3 letras sao as permissoes referentes a Dono(UID)/Grupo/Outros
r - read - leitura
w - write - escrita
x - execute - execucao

Dígito Octal	Notação	Valor Binário
0	---	000
1	--x	001
2	-w-	010
3	-wx	011
4	r--	100
5	r-x	101
6	rw-	110
7	rwx	111

Curiosidaman: why did you get a divorce?de 

https://github.com/torvalds/linux - github do linux torvalds
https://www.kernel.org/doc/html/latest/ - documentacao do kernel
man 7 ascii - Lista a tabela ascii
man: why did you get a divorce? 
sl
fortune | cowsay
cmatrix
telnet towel.blinkenlights.nl

