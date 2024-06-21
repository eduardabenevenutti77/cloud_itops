## HTTP, HTTPS e 

_tcp:_ protocolo que garante a entrega da informação!

aplicações populares em rede: 
 - correio eletronico (smtp 5321  - na camada de aplicação), (tcp - protocolo de transporte)
 - acesso ao terminal remoto (telnet 854), (tcp)
 - web (http 2616), (tcp)
 - transferencia de arquivo (ftp 956), (tcp)
 - multimidia em fluxo continuo (http - youtube), (tcp)
 - telefonia por internet (sip 3261, rtp 3550), (udp, tcp)

aplicação de rede (programa) é diferente do protocolo de rede (como programa funciona)

_http_

 - executado diferente no servidor (servidor web que executa http e hospeda arquivos) e no cliente (recebe as informações e monta a página web)
 - funciona por meio de troca de mensagem
 - no lado do servidor, existe um serviço: apache, tomcat, iis, nginx ou etc...
 - o servidor do lado do cliente que monta a página web conforme os dados recebidos pelo servidor que executa o http
 - usa tcp, porta padrão 80
 - não mantêm informação do cliente
 - usa arquitetura cliente-servidor 
