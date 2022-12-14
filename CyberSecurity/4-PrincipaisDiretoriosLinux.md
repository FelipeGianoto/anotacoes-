<h1> Diretórios do Linux </h1>

-/bin
Todos os comandos q podem ser executados por qualquer usuário 

-/boot
Diretório de bootagem do sistema operacional(arquivos necessários para inicializar o sistema linux fica dentro desse diretório)

-/dev
Pseudoarquivos(arquivos q representam periféricos, por exemplo, impressora,  placa de som, pendrive, disco rigido, web cam)

-/etc
Configuração dos principais serviços 

-/home
Diretórios de usuários equivalente a pasta de user do windows 

-/lib e /lib64
Bibliotecas dos sistema

-/lost+found
(Achados e perdidos)Arquivos corrompidos q podem ser resgatados

-/media
Cdrom 

-/opt
Diretório opcional de instalação 

-/proc
Possui pseudo-arquivos, se precisar saber alguma configuração de processador, memoria,(hardware fisicos)

-/root
Diretório home do super usuário 

-/rub
Processos (todo programa q se executa no sistema operacional)

-/sbin
Comandos específicos para o root

-/srv
Serviços de sistema

-/sys
Guarda configuração para dispositivos USB

-/usr
Onde geralmente fica instalado os programas no linux equivalente aos arquivos de programa do windows

-/var
Arquivos de tamanho variavel(banco de dados, logs de sistema)

- Ls -lah / 
- arquivos q começam com d são diretórios e os q começam com l sao links

-drwx 
R = read
W = write
X = execute

Os 3 primeiros representam as permissões do dono do arquivo q pode ser visto ao lado(root)

Do 3 ao 6 representa a permissão do grupo sobre o arquivos 

E os 3 últimos permissão de todos os usuários 

Os números são quantos arquivos tem dentro dele


-pseudo-arquivos  em c são arquivos em carácteres 
e em b são arquivos em bytes
