# HDFS basic commands

##Lista conteúdo de diretório
$ hdfs dfs -ls -R /

##Copia arquivo do sistema local para o HDFS
$ hdfs dfs -put [caminho origem]/arquivo [caminho destino]

##Move arquivo ou diretório do sistema local para HDFS
$ hdfs dfs -mv [caminho origem]/arquivo [caminho destino]

##Remove arquivo ou pasta
$ hdfs dfs -rm [caminho arquivo]/arquivo

##Verifica o tamanho do arquivo
$ hdfs dfs -du [caminho arquivo]/arquivo

##Exibe o conteúdo do arquivo
$ hdfs dfs -cat [caminho arquivo]/arquivo

##Cria um diretório
$ hdfs dfs -mkdir [caminho]

##Remove diretório
$ hdfs dfs -rmdir -R [caminho]

##Mostra parte final do arquivo
$ hdfs dfs -tail [caminho arquivo]/arquivo

##Conta número de diretórios do arquivo
$ hdfs dfs [caminho arquivo]/arquivo

##Altera o fator de replicação de um arquivo
$ hdfs dfs -setrep 3 [caminho arquivo]/arquivo

##Informa estatísticas do arquivo ou diretório
%F = tipo
%n = nome
%r = fator de replicação
%d = data de modificação
$ hdfs dfs -stat %F [caminho arquivo]/arquivo

##Verifica estado do sistema de arquivos
$ hdfs dfs -fsck /
