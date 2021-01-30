---
title: Visão geral da API de comunicações na nuvem
description: As APIs de comunicações na nuvem do Microsoft Graph adicionam uma nova dimensão à forma como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados à comunicação, como chamada e reuniões online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 572ce19e14779615ac8db514101df7d944b1d819
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059592"
---
# <a name="cloud-communications-api-overview"></a>Visão geral da API de comunicações na nuvem
As APIs de comunicações na nuvem do Microsoft Graph adicionam uma nova dimensão à forma como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados à comunicação, como chamada e reuniões online. Ampliar seus negócios agilizando a forma como você responde às necessidades dos seus clientes e como seus funcionários colaboram entre si.

## <a name="why-integrate-with-the-cloud-communications-apis"></a>Por que se integrar às APIs de comunicações na nuvem?

Descubra os benefícios de usar APIs de comunicações na nuvem para criar aplicativos de serviço[(bots).](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)

### <a name="handle-incoming-calls"></a>Lidar com chamadas de entrada

Às vezes, pode ser difícil quando os funcionários recebem muitas chamadas comerciais e não é possível, nem produtivo, atender a todas elas. Um bot pode servir como um assistente de front-desk e lidar com essas chamadas rejeitando o que parece ser chamadas de spam e redirecionando (encaminhando) chamadas específicas para um número diferente.

Você pode usar as APIs de comunicações na nuvem para:

- Fazer com que um [usuário ligue para um bot](/graph/api/application-post-calls?view=graph-rest-1.0) por meio de VoIP.
- Fazer com que um bot [redirecione a chamada](/graph/api/call-redirect?view=graph-rest-1.0) de entrada para o agente apropriado, se necessário.
- Ter uma resposta [de](/graph/api/call-answer?view=graph-rest-1.0) bot [ou rejeitar](/graph/api/call-reject?view=graph-rest-1.0) a chamada.


### <a name="simplify-the-customer-service-experience"></a>Simplificar a experiência de atendimento ao cliente
Se você possui um grande serviço de helpdesk ou uma pequena loja, pode ser difícil lidar com várias solicitações de clientes, especialmente se você não tiver qualquer contexto do problema que eles estão tentando resolver com antecedência. Lidar com chamadas de entrada de clientes por meio de um sistema **de** Resposta interativa de voz (IVR), onde um bot inicialmente interagirá com eles.

Quando um cliente é solicitado a responder pelo bot, ele pode pressionar uma tecla no teclado correspondente à seleção. O bot pode coletar a multifrequência de tom de discagem (DTMF) do cliente.

Você pode usar as APIs de comunicações na nuvem para criar um bot que:

- [Atende uma chamada](/graph/api/call-answer?view=graph-rest-1.0) de um cliente.
- [Reproduz um prompt para](/graph/api/call-playprompt?view=graph-rest-1.0) informar e solicitar uma seleção ao cliente.
- [Assina um tom para](/graph/api/call-subscribetotone?view=graph-rest-1.0) coletar a DTMF de um cliente.
- [Transfere um cliente](/graph/api/call-transfer?view=graph-rest-1.0) para um agente.
- [Encerra uma chamada](/graph/api/call-delete?view=graph-rest-1.0) com um cliente.

![Imagem de um bot fornecendo opções para transferência de chamada](images/communications-ivr-transfer.png)

Para criar uma interação mais inteligente entre seus clientes e seu bot, quando um cliente for solicitado a responder, ele poderá falar diretamente sobre o que precisa de ajuda.

A integração com um serviço de processamento de linguagem natural significa que a fala do cliente pode ser analisada por seu significado. Em seguida, o bot pode responder às necessidades do cliente de acordo.

>**Observação:** Você não pode gravar ou persistir conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia. Certifique-se de que você está em conformidade com as leis e os regulamentos da sua área em relação à proteção de dados e confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

Você pode usar as APIs de comunicações na nuvem para criar um bot que:

- [Atende uma chamada](/graph/api/call-answer?view=graph-rest-1.0) de um cliente.
- [Reproduz um prompt para](/graph/api/call-playprompt?view=graph-rest-1.0) informar e solicitar que o cliente fale.
- [Grava um pequeno clipe de áudio](/graph/api/call-record?view=graph-rest-1.0) de um cliente que fala.
- [Reproduz um prompt](/graph/api/call-playprompt?view=graph-rest-1.0) com a resposta apropriada para o cliente, após a análise da fala.

![Imagem de um bot que solicita que um usuário dê uma resposta de voz](images/communications-ivr.PNG)

### <a name="collaborate-through-group-calls"></a>Colaborar por meio de chamadas de grupo
Permita que os usuários se envolvam com colegas de trabalho ou clientes criando uma chamada de grupo para que todos possam contribuir com a conversa.

Você pode usar as APIs de comunicações na nuvem para criar um bot que:

- [Cria uma chamada de grupo](/graph/api/application-post-calls?view=graph-rest-1.0#example-3-create-a-group-call-with-service-hosted-media) com vários participantes.
- [Convida outro bot ou usuário para](/graph/api/participant-invite?view=graph-rest-1.0) uma chamada de grupo existente.
- [Ins junta-se a uma chamada de grupo](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media) existente como um bot.
- [Lista os participantes na](/graph/api/call-list-participants?view=graph-rest-1.0) chamada de grupo.
- [Silencia outro participante.](/graph/api/participant-mute?view=graph-rest-1.0)

### <a name="send-reminders-reliably"></a>Enviar lembretes de forma confiável
Para permitir que os usuários enviem aos clientes um lembrete para um compromisso ou um lembrete para uma data limite de pagamento que está se aproximando, você pode fazer um bot ligar para o cliente automaticamente. <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

Você pode usar as APIs de comunicações na nuvem para criar um bot que:

- [Liga para um cliente](/graph/api/application-post-calls?view=graph-rest-1.0) no Teams.
- [Reproduz um prompt gravado](/graph/api/call-playprompt?view=graph-rest-1.0) para servir como lembrete.
- [Encerra a chamada.](/graph/api/call-delete?view=graph-rest-1.0)


### <a name="set-up-online-meetings"></a>Configurar reuniões online
Seja agendando uma reunião entre um médico e um paciente ou entre um usuário e seus relatórios diretos, você pode criar soluções que gerem reuniões nas que os usuários podem confiar. Para maior flexibilidade, os usuários podem ligar para outros usuários e convidá-los para a reunião enquanto ela está em andamento.

Você pode usar as APIs de comunicações na nuvem para:

- Fazer com que um [usuário crie uma reunião online.](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)
- Fazer com que [um usuário recupere os detalhes](/graph/api/onlinemeeting-get?view=graph-rest-1.0) de uma reunião online.
- Fazer um bot ou um usuário [ingressar em uma reunião online.](/graph/api/application-post-calls?view=graph-rest-1.0#example-5-join-scheduled-meeting-with-service-hosted-media)

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [APIs de comunicações na nuvem no Microsoft Graph (v1.0)](/graph/api/resources/communications-api-overview?view=graph-rest-1.0)
- [APIs de comunicações na nuvem no Microsoft Graph (beta)](/graph/api/resources/communications-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- Use bots para [começar.](cloud-communications-get-started.md)
- Saiba mais sobre [chamadas,](cloud-communications-calls.md) [mídia](cloud-communications-media.md)e [reuniões online.](cloud-communications-online-meetings.md)
- Exibir os limites de uso [da](throttling.md#cloud-communication-service-limits)API.
- Saiba como gerenciar [números de telefone](cloud-communications-phone-number.md) para seus bots.

## <a name="see-also"></a>Confira também

- [Permissões delegadas e de aplicativo](/azure/active-directory/develop/v1-permissions-and-consent)
- [Permissões de chamadas](./permissions-reference.md#calls-permissions)
- [Permissões de reunião online](./permissions-reference.md#online-meetings-permissions)
- [Exemplos de comunicações na nuvem](https://github.com/microsoftgraph/microsoft-graph-comms-samples)
