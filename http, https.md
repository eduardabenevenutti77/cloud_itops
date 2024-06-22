## HTTP & HTTPS | FTP 💻

> _tcp:_ protocolo que garante a entrega da informação!

aplicações populares em rede: 
 - correio eletronico (smtp 5321  - na camada de aplicação), (tcp - protocolo de transporte)
 - acesso ao terminal remoto (telnet 854), (tcp)
 - web (http 2616), (tcp)
 - transferencia de arquivo (ftp 956), (tcp)
 - multimidia em fluxo continuo (http - youtube), (tcp)
 - telefonia por internet (sip 3261, rtp 3550), (udp, tcp)

> aplicação de rede (programa) é diferente do protocolo de rede (como programa funciona)

_http_

 - executado diferente no servidor (servidor web que executa http e hospeda arquivos) e no cliente (recebe as informações e monta a página web)
 - funciona por meio de troca de mensagem
 - no lado do servidor, existe um serviço: apache, tomcat, iis, nginx ou etc...
 - o servidor do lado do cliente que monta a página web conforme os dados recebidos pelo servidor que executa o http
 - usa tcp, porta padrão 80
 - não mantêm informação do cliente
 - usa arquitetura cliente-servidor 

_https_

 - usa tcp, porta 443
 - usa ssl (sistema que fornece privacidadade, integridade e autenticação)
 - garante transporte seguro, mas não garante que o servidor é seguro
 - evita o main-in-the-middle
 - ssl analisa a identidade do servidor com base no certificado

_ftp_

 - protocolo de transferencia de arquivo
 - usa tcp, portas: 21 (controle), 20 (transf)

_arquitetura_de_redes_

 - mainframes: caros, otimizar recursos e menor flexibilidade de usuário
 - pcs anos 80: rede local, computação cliente/servidor, hegemônica, peer to peer (p2p)
 - virtualização: iniciou nos anos 60, perdeu força pelos pcs, ganhou forças no 90 com o aumento do processamento
 - a rede cliente/servidor era interna, rede entre organizações custava caro
 - computação em núvem nos anos 2000 facilitava o TI e a infra como um serviço
 - internet e protocolos possibilita extranets (mais baratos)

> p2p - descentralização (divisão para vários servidores)

_cliente-servidor_
 
 - um host (servidor) sempre em funcionamento
 - atende as requisições de outros servidores (clientes)
 - o servidor possui endereço fixo conhecido e fácil de encontrar

_peer-to-peer_

 - bom custo benefício
 - tem problema na largura de banca

cluster: sistema com dois ou mais computadores que trabalham em conjunto com objetivo de processar uma tarefa
 > atividades como processamento são dividas entre as máquinas que executam de maneira simultânea

grid: objetivo parecido com cluster, não há um ponto central de distribuição, mais democrático e cooperativo, pode ter compartilhamento geograficamente distante

computação em nuvem: recursos de computadores e servidores compartilhados por meio da internet, segue o principio de grids
> revolucionou a maneira em que as infraestruturas são gerenciadas e acessadas, paga pelo recurso alocado e reservado