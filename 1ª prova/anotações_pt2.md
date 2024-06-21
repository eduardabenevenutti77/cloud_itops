camada tcp: transporte - orientado a conexão 
como o tcp faz para controlar dados recebidos: seq e ack
ipv4: 
 - endereçamento de redes, identificação e comunicação de dispositivos
 - 4 blocos de 8 bits
 é divido em dois tipos:
  1º - válidos;
  2º - locais (interno);
REVISÃO - 12/04
IPV4: 
  mecanismo de endereçamento na camada de rede, identificação e comunicação entre dispositivos de rede, 
formado por 4 blocos de 8 bits (32), dividido em endereços: válidos e locais (internos);
  representado por decimais de 0 - 255, são transformado em binários ao serem processados
  estrutura hierárquica: redes e hosts
  diferentes identificadores para diferentes redes!
  na mesma rede os identificadores são iguais
  cada host tem um identificador exclusivo!
pq o classe de padrão parou de existir? por causa da quantidades de números a serem usados e a quantidade de ip's a serem usados
máscara de rede: cria redes de diferente tamanhos, ao trocar o valor do penúltimo bloco por 0 ou 1 - ajusta a tamanho da rede
review:
- quando maior for a parte de rede, menor será a parte de host!
- a máscara permite personalizar o tamanho da rede
- em binário onde a máscara está tudo em 1111111 -> rede || se está tudo 000000000 -> host
- mais bits = mais hosts -> menos bits = menos hosts

placa de rede atual:
 operação and: conta matematica com os bits 
 1 and 1 = 1
 1 and 0 = 0
 0 and 1 = 0
 0 and 0 = 0
endereço privados (internos):
 - usados apenas em rede locais, começam com 10 | 192.168 ou 172.16 até 172.31
 - roteadores de grandes redes são configurados para ignorar 
maneira de economizar ip - ofertar de maneira dinamica, conforme for aparecendo a necessidade de uso

limitações do IPv4:
 - falta de endereços IP;
 - falta de conectividade de ponta a ponta - NAT;
 - expensão da tabela de roteamento da Internet;

solução IPv6:
 - aumento de espaço de endereços - 128 bits (340 undecilhões de endereços);
 - melhoria no tratamento de pacotes;
 - evita problemas relacionados ao NAT;

transição de IPv4 para IPv6:
 - roda pilhas duplas (ipv4 e ipv6 simultaneamente) -> + usado em dispositivos de redes (a máquina ela pega o IPV que estiver disponível)
 - transpote ipv6 dentro do pacote ipv4 (tunelamento) -> há um intermediário entre os dois IPV's
 - converte pacotes de ipv4 para ipv6 - vice-versa (tradução) 

- atualmente cada máquina tem um IP único e exclusivo (IPV6);
- geralmente as máquinas oferecem os dois tipos (IPV4/IPV6);
- o ipv6 é extremamente necessário!

Representação IPV6:
 - 128 bits ao total
 - 4 dígitos em cada grupo hexadecimal
 - 8 grupos hexadecimal
 - tem prefixo de rede (1ª representa a rede, 2ª representa o host)
 - se tiver vários dígitos 0 - podemos omitir por ":" -> 2804:bd8:fa0:0:0:0:07344 - 2804:bd8:fa0::7344

Representação IPV6 - OUTROS TIPOS:
 - link local (criado automaticamente usando o prefixo FE80:/64 para uso local quando não há ipv6 disponível do provedor)
 - unique local address (ula) - endereço com probabilidade de ser globalmente único, usado só para comunicação local FC000 - FDFF::/7
 - não especificado - ausência de endereço ::/128
 - loopback - localhost ::1/128

configuração IPV6:
 - o modem dá a parte da rede, a máquina delimita a parte do host conforme o sistema operacional!
 - a máquina deve fazer 16 bits para o host
 - o windowns realiza de forma aleatoria