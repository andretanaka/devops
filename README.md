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
ps 
ps -ef | grep [nome do processo]
```

> -a = Exibe todos os processos existentes.

> -e = Exibe as variáveis de ambiente relacionadas aos processos.

> -f = Exibe a árvore de execução dos processos.

> -l = Exibe mais campos no resultado.

> -m = Exibe a quantidade de memória ocupada por cada processo.

> -u = Exibe o nome do usuário que iniciou determinado processo e a hora em que isso ocorreu.

> -x = Exibe os processos que não estão associados a terminais.


Terminar um processo

```
kill -9 [PID/Nome do processo]
killall -9 [PID/Nome do processo]
```

<h2>Sistema de permissões</h2>
<b>-rwxrwxrwx</b>

<h4>Primeiro caractere = Natureza do arquivo:</h4>
<table>
  <thead>
    <th>Caractere</th>
    <th>Significado</th>
  </thead>
  <tbody>
    <tr>
      <td>-</td>
      <td>Arquivo regular</td>
    </tr>
    <tr>
      <td>d</td>
      <td>Arquivo de diretório</td>
    </tr>
    <tr>
      <td>l</td>
      <td>Link</td>
    </tr>
    <tr>
      <td>b</td>
      <td>Arquivos de dispositivo orientado a bloco</td>
    </tr>
    <tr>
      <td>c</td>
      <td>Arquivos de dispositivo orientado a caractere</td>
    </tr>
    <tr>
      <td>s</td>
      <td>Socket</td>
    </tr>
    <tr>
      <td>p</td>
      <td>Named pipe (ou FIFO)</td>
    </tr>
  </tbody>
</table>

<h4>Os próximos 3 grupos de 3 caracteres são as permissões referentes a Dono(UID)/Grupo/Outros</h4>
<table>
  <thead>
    <th>Caractere</th>
    <th>Significado</th>
    <th>Função</th>
  </thead>
  <tbody>
    <tr>
      <td>r</td>
      <td>Read</td>
      <td>Leitura</td>
    </tr>
    <tr>
      <td>w</td>
      <td>Write</td>
      <td>Escrita</td>
    </tr>
    <tr>
      <td>x</td>
      <td>Execute</td>
      <td>Execução</td>
    </tr>
  </tbody>
</table>

É possível alterar as permissões de um arquivo através do seguinte comando:

```
chmod -R [u/g/o][+/-][r/w/x] arquivo/diretório
Exemplo:
chmod -R u+rwx g-rwx o+rwx arquivo/diretorio
chmod -R 777 arquivo diretorio
```
A o primeiro grupo de opções ([u/g/o]) é referente ao tipo de usuário, onde:
<table>
  <thead>
    <th>Caractere</th>
    <th>Tipo de usuário</th>
  </thead>
  <tbody>
    <tr>
      <td>u</td>
      <td>Dono</td>
    </tr>
    <tr>
      <td>g</td>
      <td>Grupo</td>
    </tr>
    <tr>
      <td>o</td>
      <td>Outros</td>
    </tr>
  </tbody>
</table>

O segundo grupo de opções ([+/-]) indica a inclusão (+) ou remoção (-) das permissões indicadas no próximo grupo de opções ([r/w/x]).


Dígito Octal	Notação	Valor Binário
0	---	000
1	--x	001
2	-w-	010
3	-wx	011
4	r--	100
5	r-x	101
6	rw-	110
7	rwx	111

chmod -R u+rwx g-rwx o+rwx arquivo/diretorio
chmod -R 777 arquivo diretorio

chown novousuario arquivo/diretorio
chown novousuario:novogrupo arquivo/diretorio
chown :novogrupo arquivo/diretorio

Curiosidaman: why did you get a divorce?de 

https://github.com/torvalds/linux - github do linux torvalds
https://www.kernel.org/doc/html/latest/ - documentacao do kernel
man 7 ascii - Lista a tabela ascii
man: why did you get a divorce? 
sl
fortune | cowsay
cmatrix
telnet towel.blinkenlights.nl

