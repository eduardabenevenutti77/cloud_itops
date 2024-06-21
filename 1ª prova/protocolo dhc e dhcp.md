o que é?
 - atribui endereços IPS automaticamente
 - tem uma lista de endereços disponíveis

funcionamento:
  - um software com endereço automáticos que ao iniciar encaminha por meio de broadcast, com isso ele responde com o IP disponível e outros dados necessários
  - envia um broadcast (uma mensagem para geral) para realizar a busca de ip para validar as informações pedidas pelo cliente

  - caso tenha mais de dhcp, eles precisam estar conectados!

  cliente dhcp: pedem endereço
  servidor dhcp: gerenciam os endereços

 [DHCP FUNCTION - IMAGE 📓](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.learncisco.net%2Fcourses%2Ficnd-1%2Flan-connections%2Frouter-as-a-dhcp-server.html&psig=AOvVaw02kv_kXErItW4W-kGakTtr&ust=1716078433342000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCMiPosj4lYYDFQAAAAAdAAAAABAJ)

consessões: 
 - empresta um IP com tempo para expirar
 - dura em média 6 ou 8 dias, mas por padrão 8 horas
 - clientes devem renovar o pedido (o próprio windows realiza isso)
 - em 50% do prazo de entrega o servidor entra em contato com dhcp para renovar o pedido
 - em 87,5% do tempo realiza novamente o pedido de renovação, se no 50% do tempo não obteve resposta
 - quando o dispositivo desliga, o IP é retornado ao DHCP (liberando o endereço)

DHCPv6:
 - tem menos funções
 - usamos para quando queremos manter o registro
 - usa ipv6 (não tem broadcast)
 - tem 3 modelos de funcionamento (1º não necessita do dhcp, só entrega o prefixo o solicitante complementa SLAAC, 2º stateless (cliente só solicita alguns parametros para conf)/statefull ,3º)

 endereço de broadcast: 255.255.255.255

 métodos de dhcp:
  discover - emite uma mensagem broadcast
  offer - responde com as config necessárias e um IP
  request - responde com uma solicitação do endereço ip da mensagem
  ack - se o endereço estiver livre, emite uma mensagem de confirmação