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
> -l = traz detalhes dos arquivos como datas de criação, permissões, nome de proprietário e grupo, e tamanho.

> -a ou -all = inclui os arquivos ocultos na listagem

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

Criando um arquivo

```
touch texto.txt          - Cria um arquivo vazio
> texto.txt              - Cria um arquivo vazio. Se o arquivo existir, esse comando limpa o conteúdo do arquivo.
echo "texto" > texto.txt - Cria o arquivo texto.txt com o conteúdo "texto".
vim texto.txt            - Abre uma instância do vim editando um arquivo vazio chamado texto.txt.
```
Concaternar um texto no final do arquivo

```
echo "texto" >> texto.txt - concatena no final do arquivo
```

Exibe o conteúdo de um arquivo

```
cat texto.txt
```

Criando um alias

```
alias [alias]="[comando]"
```

Removendo um alias

```
unalias [alias]
```

Exibir os processos em execução

```
ps -ef - exibe os processos em execucao sem infos de processamento e memoria usados
```

> -a = Exibe todos os processos existentes.
> -e = Exibe as variáveis de ambiente relacionadas aos processos.
> -f = Exibe a árvore de execução dos processos.
> -l = Exibe mais campos no resultado.
> -m = Exibe a quantidade de memória ocupada por cada processo.
> -u = Exibe o nome do usuário que iniciou determinado processo e a hora em que isso ocorreu.
> -x = Exibe os processos que não estão associados a terminais.


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

