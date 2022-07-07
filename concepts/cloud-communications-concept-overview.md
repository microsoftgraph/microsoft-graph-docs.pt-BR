---
title: Visão geral da API de comunicações na nuvem
description: Use a API de comunicações na nuvem no Microsoft Graph para criar bots que lidam com chamadas de entrada, colaboram por meio de chamadas em grupo, enviam lembretes e configuram reuniões.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 38c9ed8b4d12f4962f0e31b4ac1f730969e46c2b
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666862"
---
# <a name="cloud-communications-api-overview"></a>Visão geral da API de comunicações na nuvem

A API de comunicações na nuvem no Microsoft Graph adiciona uma nova dimensão à maneira como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados à comunicação, como chamadas e reuniões online. Expanda seus negócios agilizando a maneira como você responde às necessidades de seus clientes e como seus funcionários colaboram entre si.

Para descobrir os benefícios de usar a API de comunicações na nuvem para criar aplicativos de serviço ([bots](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html?q=create%20bot)), confira as seções a seguir.

## <a name="handle-incoming-calls"></a>Manipular chamadas de entrada

Às vezes, pode ser difícil quando os funcionários recebem muitas chamadas comerciais e não é possível, nem produtivo, atender a todos eles. Um bot pode servir como um assistente de front-desk e lidar com essas chamadas rejeitando o que parece ser chamadas de spam e redirecionando (encaminhando) chamadas específicas para um número diferente.

Você pode usar a API de comunicações na nuvem para:

- Fazer com que um [usuário chame um bot](/graph/api/application-post-calls) por meio de VoIP.
- Fazer com que um bot [redirecione a chamada de](/graph/api/call-redirect) entrada para o agente apropriado, se necessário.
- Ter uma resposta [de bot](/graph/api/call-answer) ou [rejeitar](/graph/api/call-reject) a chamada.


## <a name="simplify-the-customer-service-experience"></a>Simplificar a experiência de atendimento ao cliente

Seja você o dono de um grande serviço de assistência técnica ou de uma pequena vitrine, pode ser difícil lidar com várias solicitações de clientes, especialmente se você não tiver nenhum contexto do problema que eles estão tentando resolver com antecedência. Manipular chamadas de entrada de clientes por meio de um sistema IVR ( **Resposta** interativa de voz), em que um bot inicialmente interagirá com eles.

Quando um cliente é solicitado a fornecer uma resposta do bot, o cliente pode pressionar uma tecla em seu teclado que corresponda à sua seleção. Em seguida, o bot pode coletar o DTMF (multi-frequency) de tom de discagem do cliente.

Você pode usar a API de comunicações na nuvem para criar um bot que:

- [Atende a uma chamada](/graph/api/call-answer) de um cliente.
- [Reproduz um prompt para](/graph/api/call-playprompt) informar e solicitar uma seleção a um cliente.
- [Assina um tom para](/graph/api/call-subscribetotone) coletar o DTMF de um cliente.
- [Transfere um cliente](/graph/api/call-transfer) para um agente.
- [Encerra uma chamada](/graph/api/call-delete) com um cliente.

![Imagem de um bot fornecendo opções para transferência de chamada](images/communications-ivr-transfer.png)

Para criar uma interação mais inteligente entre seus clientes e seu bot, quando um cliente for solicitado a fornecer uma resposta, ele poderá falar diretamente sobre o que precisa de ajuda.

A integração com um serviço de processamento de idioma natural significa que a fala do cliente pode ser analisada para seu sentimento. Em seguida, o bot pode responder à necessidade do cliente adequadamente.

> [!NOTE]
> Você não pode gravar ou persistir conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia. Verifique se você está em conformidade com as leis e regulamentos da sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

Você pode usar a API de comunicações na nuvem para criar um bot que:

- [Atende a uma chamada](/graph/api/call-answer) de um cliente.
- [Reproduz um prompt para](/graph/api/call-playprompt) informar e solicitar que o cliente fale.
- [Grava um curto clipe de áudio](/graph/api/call-record) de um cliente que fala.
- [Reproduz um prompt](/graph/api/call-playprompt) com a resposta apropriada para o cliente, depois que sua fala é analisada.

![Imagem de um bot que solicita que um usuário forneça uma resposta de voz](images/communications-ivr.PNG)

## <a name="collaborate-through-group-calls"></a>Colaborar por meio de chamadas de grupo
Permitir que os usuários se envolvam com colegas de trabalho ou clientes criando uma chamada em grupo para que todos possam contribuir para a conversa.

Você pode usar a API de comunicações na nuvem para criar um bot que:

- [Cria uma chamada em grupo](/graph/api/application-post-calls#example-3-create-a-group-call-with-service-hosted-media) com vários participantes.
- [Convida outro bot ou usuário para](/graph/api/participant-invite) uma chamada de grupo existente.
- [Ingressa em uma chamada de grupo existente](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media) como um bot.
- [Lista os participantes na](/graph/api/call-list-participants) chamada de grupo.
- [Ativa o mudo de outro participante](/graph/api/participant-mute).

## <a name="send-reminders-reliably"></a>Enviar lembretes de forma confiável
Para permitir que os usuários enviem aos clientes um lembrete para um compromisso ou um lembrete para um prazo de pagamento que está se aproximando, você pode fazer com que um bot chame o cliente automaticamente. <!--If the customer misses the call, it will leave a voicemail with the automated message. (Add this back once bot to PSTN calling works)-->

Você pode usar a API de comunicações na nuvem para criar um bot que:

- [Chama um cliente](/graph/api/application-post-calls) no Teams.
- [Reproduz um prompt gravado](/graph/api/call-playprompt) para servir como um lembrete.
- [Encerra a chamada](/graph/api/call-delete).


## <a name="set-up-online-meetings"></a>Configurar reuniões online
Seja agendando uma reunião entre um médico e um paciente ou entre um usuário e seus relatórios diretos, você pode criar soluções que gerem reuniões nas quais os usuários possam confiar. Para maior flexibilidade, os usuários podem chamar outros usuários e convidá-los para a reunião enquanto ela está em andamento.

Você pode usar a API de comunicações na nuvem para:

- Fazer com que um [usuário crie uma reunião online](/graph/api/application-post-onlinemeetings).
- Fazer com que [um usuário recupere os detalhes](/graph/api/onlinemeeting-get) de uma reunião online.
- Fazer com que um bot ou um usuário [ingresse em uma reunião online](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media).

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de comunicações na nuvem no Microsoft Graph v1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true)
- [API de comunicações na nuvem no Microsoft Graph beta](/graph/api/resources/communications-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Próximas etapas

- Use bots para [começar](cloud-communications-get-started.md).
- Saiba mais sobre [chamadas](cloud-communications-calls.md), [mídia](cloud-communications-media.md) e [reuniões online](cloud-communications-online-meetings.md).
- Exiba os limites de [uso da](throttling-limits.md#cloud-communication-service-limits) API.
- Saiba como gerenciar [números de telefone](cloud-communications-phone-number.md) para seus bots.

## <a name="see-also"></a>Confira também

- [Permissões delegadas e de aplicativo](/azure/active-directory/develop/v1-permissions-and-consent)
- [Permissões de chamadas](./permissions-reference.md#calls-permissions)
- [Permissões de reunião online](./permissions-reference.md#online-meetings-permissions)
- [Exemplos da API de comunicações na nuvem](https://github.com/microsoftgraph/microsoft-graph-comms-samples)
