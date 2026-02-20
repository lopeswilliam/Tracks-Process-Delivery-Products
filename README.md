# Tracks-Process-Delivery-Products

**1 - **Cliente, acessa a interface via mobile ou Web.

**2 - **Executa o fluxo da transacao.

2.1 - Gera o numero do pedido.

**3 -** publica no topic e depois consome a informação, envia ACK.

**4 - **Obtem a informaçao, grava no bd.

4.2 - Notifica o usuario consumer.

**5 - **User Delivery, pega a notificaçao,  executa o fluxo de entrega.

**6 -** Obtem a informaçao, grava no bd - vendor.

6.1 - As informações sao postadas no topic, e depois consumidas, envia ACK.

**7 - **Notifica o usuario que o produto será entregue em um determinado tempo.

7.1 - Notifica o inicio e o caminho, que encontra se o pedido.

7.2 - Qualquer movimentaçao que venha a ocorrer, o usuario vendor notifica o usuario consumer, on the time, atraves de mensagem.

**8 - **Até o Cliente receber o produto, ou nao, sempre terá o motivo da nao entrega do produto.

**9 - **User Business utiliza a ferramenta de analytics, para verificar o business, operacoes, delivery, etc... 
