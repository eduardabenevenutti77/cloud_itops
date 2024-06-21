redes de computadores e a internet?
 - isp : provedor de serviço de internet (claro, vivo, tim), podem ser nacionais ou globais
 - isp local: provedor de serviço regional (SIM FIBRA) 

iso/osi:
 modelo osi - 7 camadas 👩‍💻: 
  as mensagens que enviamos passa por essas 7 camadas!
  - aplicação, apresentação, sessão, transporte, rede, enlace e física (camadas mais altas estão mais perto do usuário - as mais baixas estão próximas do hardware)
  - o tráfego (transformação dos informações inseridas pelo usuário em dados) nas redes acontece por pacotes
  - cada camada inclui a informações ao pacote, os dados inicias não podem sofrer alterações. cada info add é denominada de cabeçalho
  - o cabeçalho do pacote é a informação que detalha o formato dela

    camada física (1º): 
    exemplo -> MODEM
    - converte os bits em algo interpretável
    - se preocupa com o tipo, espaço e material
    - é o cara que converte um sentido para outro (de bit para ondas de rádio)
    como pode ocorrer a transmissão de 3 formas: 
      1 - simplex: um dispositivo transmite (Tx) o dado e o outro recebe (Rx) o dado transmitido (Unidirecional); 
      2 - half-duplex: walk tok, um recebe e o ou emite por vez / um sentido por vez;   
      3 - full-duplex: telefone, transmissão e recebimento de dados ao mesmo tempo.

    camada enlace (2º):
    - controle de acesso ao meio físico, detecção de erros (define meios para reconhecer erros)
    - recebe as informações enviadas pela camada física e análisa o status da informação
    - verifica se os dados não foram alterados

    camada rede (3º):
    - recebe endereço lógico, delimitado pelo administrador da rede
    - responsável pelo endereçamento e roteamento da rede - IP
    - controla a maneira que os pacotes de dados são roteados da origem até o final da operação 
    - protocolo IP
    - IP (protocolo de internet)
    - criação de caminhos para a informação chegar em determinado ponto

            - o IP é o endereço lógico - 

    camada de transporte (4ª): 
    - controle lógico dos dados
    - determina como a conexão vai acontecer
    - o uso desses modelos depende de onde/quando for utilizado
    pode ser dividido em duas partes: orientado a conexão (verfica-se a existência o destino - GARANTE A ENTRAGA) e o não orientado a conexão (não verifica a existência do destino, e de tal modo, não se preocupa com os dados enviados - SÓ ENVIA)

    camada de sessão (5º):
    - responsável pelo processo de inciar e encerrar um conexão entre hosts
    - suporte: registros de logs e tarefas de segurança
    
    camada de apresentação (6º):
    - efetua a tradução dos dados recebidos
    - conversão de código para caracteres

    camada de aplicação (7º): 
    - garante a interação humano-máquina
    - camada dos protocolos (http, ftp)

existem dispositivos que verificam camadas determinadas
quanto mais camada = mais funções

protocolo tcp: orientado a conexão

PORTAS & SEGURANÇAS: 
  - 443: https - nível de segurança superior
  - 80: http - nível de segurança menor em comparação ao 443