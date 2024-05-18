o que é?
 - atribui endereços IPS automaticamente
 - tem uma lista de endereços disponíveis

funcionamento:
  - um software com endereço automáticos que ao iniciar encaminha por meio de broadcast, com isso ele responde com o IP disponível e outros dados necessários;
 [DHCP FUNCTION - IMAGE 📓](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.learncisco.net%2Fcourses%2Ficnd-1%2Flan-connections%2Frouter-as-a-dhcp-server.html&psig=AOvVaw02kv_kXErItW4W-kGakTtr&ust=1716078433342000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCMiPosj4lYYDFQAAAAAdAAAAABAJ)

consessões: 
 - empresta um IP com tempo para expirar
 - dura em média 6 ou 8 dias, mas por padrão 8 horas
 - clientes devem renovar o pedido (o próprio windows realiza isso)
 - em 50% do prazo de entrega o servidor entra em contato com dhcp para renovar o pedido
 - em 87,5% do tempo realiza novamente o pedido de renovação, se no 50% do tempo não obteve resposta
 - quando o dispositivo desliga, o IP é retornado ao DHCP (liberando o endereço)
 - 
