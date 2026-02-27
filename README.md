# Tracks-Process-Delivery-Products

**Objetivo desta proposta de solução arquitetural**

**Demonstrar como a informação é trafegada desde a atuação do cliente consumidor, comprador até a entrega do produto. **

1 - Cliente, acessa a interface via mobile ou Web.

2 - Escolhe o produto.

2.1 - Executa o fluxo da transacao.

2.2 - Gera o numero do pedido.

3 - Publica no topic e depois consome a informação, envia ACK.

4 - Obtem a informaçao, grava no bd.

4.1 - Notifica o usuario consumer.

**4.2 - Usuario consumer, PODE CANCELAR O PEDIDO AH QUALQUER MOMENTO..**

5 - User vendor_delivery, pega a notificaçao, executa o fluxo de entrega.

5.1 - Comunicação com o cliente usuario consumer, on the time, atraves de mensagem.

6 - Obtem a informaçao, grava no bd - vendor_delivery.

6.1 - As informações sao postadas no topic, e depois consumidas, envia ACK.

7 - Notifica o usuario que o produto será entregue em um determinado tempo.

7.1 - Notifica o inicio e o caminho, que encontra se o pedido.

7.2 - Qualquer movimentaçao que venha a ocorrer, o usuario vendor_delivery notifica o usuario consumer, on the time, atraves de mensagem.

8 - Até o Cliente receber o produto, ou nao, sempre terá o motivo da nao entrega do produto.

9 - User Business utiliza a ferramenta de analytics, para verificar o business, operacoes, delivery, etc... 


**Modelo C4-MODEL**

**Tipo: CONTEXTO**

O modelo consegue exibir vários níveis de detalhes e fornece uma maneira para que os desenvolvedores de software e partes interessadas tenham compreensão do sistema sem se ater muito aos detalhes.

**Nível 1: Contexto**

O nível de contexto fornece uma visão panorâmica do sistema, identificando os principais elementos e suas interações de alto nível.

Isso inclui usuários, sistemas externos e os principais componentes do sistema em questão. 

Este desenho arquitetural faz parte de uma proposta de solução para atender uma solicitaçao de modernizar os processos disruptivos que futuramente seram implementados em uma novas proposta de modernização arquitetural.

**PROPOSTA DE SOLUCAO ARQUITETURAL GOOGLE GCP**

Está proposta de solução arquitetural tem como objetivo utilizar os recursos computacionais que o provedor  GOOGLE GCP.

Fornece para implementar o produto DELIVERY PRODUCTS, utilizando os padroes e boas praticas da solução arquitetural.
Incluindo segurança, escalabilidade, robustez, integridade da informação e consistencia dos dados.

Foram avaliados os requisitos nao funcionais e funcionais para validar a usabilidade dos recursos, aplicando todos os criterios de aceite.

O desenho arquitetural, esta sujeito a alterações.


**Tracks I.A. INNOVATION BY WILLIAM LOPES**
