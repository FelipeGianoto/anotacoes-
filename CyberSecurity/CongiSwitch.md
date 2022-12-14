<h1> Configurar Switch </h1>

-ligar cabo console no pc na porta 238 e na porta console do swtich

<h5> Comandos </h5>
Configuração inicial
1 - enable 
Ativa modo de usuário privilegiado

2 - configura terminal
Modo de configuração global

3 - hostname + (nome)
Permite q muda o nome 

4 - enable password + (senha)
Sempre q for entrar no usuário privilegiado ira pedir uma senha

——-—— termino de configuração inicial ————

5 - configure terminal
modo de configuração global

6 - line console 0
porta console numero 1, pois comeca a contar do 0

7 - password (senha)
toda vez q for conectar no dispositivo vai pedir senha

8 - login
Ativa essa senha automaticamente 

9 - exit (duas vezes pra testar)
Quando voltar para o usuário  básico  e apertar enter vai pedir a senha

————-—-Senha de acesso via terminal—————

-pode definir quantidades de acessos ao dispositivo

10 - configure terminal
modo de configuração global

11 - line vty 0 15
0 a 15 pois você permite apenas 16 conexões de linha

12 - password + (senha)
sempre q entrar no vty

13 - login 
ativa a senha

——————————— testes ——————————

14 - exit
Ate voltar pra usuário privilegiado 

15 - show running-config
mostra todas as configurações iniciais do dispositivo 

—— Configuração de criptografia das senhas —-

16 - configure terminal
configuração global

17 - service password-encryption
todas as senhas serão encriptadas

18 - show running-config
para observar as senha criptografadas 

————-————-Configurar WLAN————————

19 - enter 
colocar senha de acesso criada no item 7

20 - enable
colocar senha criada no item 4 

21 - configure terminal

22 - interface vlan 1 
entra na interface de configuração da vlan 1 

23 - ip adress 192.168.0.100 255.255.255.0 
IP + máscara  de rede

24 - no shutdown
todo dispositivo de rede q precisar ser colocado uma configuração de interface é preciso q coloque esse comando para ligar a interface

25 - exit

26 - show running-config
verifica as configurações 

————————Configurar no pc————————-
27 - abrir o prompt de comando

28 - telnet 192.168.0.100 
ira cair no sistema de gerenciamento do cisco IOS do switch, pedindo a senha do item 12

29 - enable
colocar senha do item 4 

30 - 
