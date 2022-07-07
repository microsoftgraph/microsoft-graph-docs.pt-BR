---
title: Trabalhando com a API de comunicações na nuvem no Microsoft Graph
description: A API de comunicações na nuvem do Microsoft Graph adiciona uma nova dimensão à maneira como seus aplicativos e serviços podem interagir com os usuários, habilitando os recursos de voz e vídeo.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
ms.localizationpriority: high
ms.openlocfilehash: 2b6748d9e2d8f3a0720053083daa33c751554150
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668059"
---
# <a name="working-with-the-cloud-communications-api-in-microsoft-graph"></a>Trabalhando com a API de comunicações na nuvem no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API de comunicações na nuvem do Microsoft Graph adiciona uma nova dimensão à maneira como você ou sua organização podem interagir com outros usuários, habilitando os principais recursos e funções de comunicação de seus aplicativos e serviços. Você pode usar esta API para criar e receber chamadas, criar e recuperar coordenadas da reunião e verificar a presença dos usuários.

Você pode usar a API de comunicações na nuvem para criar aplicativos de serviço (bots) que atuam como participantes de uma chamada, criam e recuperam reuniões em nome dos usuários e verificam a disponibilidade e a atividade de presença.
Essa API fornece funcionalidade de chamada, bem como a capacidade de criar e recuperar reuniões online. Você pode usar aplicativos de serviço (bots) com esta API, onde o bot pode atuar como participante de suas chamadas de VoIP ou reuniões do Microsoft Teams, por exemplo.

## <a name="authorization"></a>Autorização

É necessária uma das seguintes [permissões](/graph/permissions-reference#calls-permissions) para acessar a API de comunicações na nuvem. Essas permissões precisam ser concedidas pelo administrador.

| Cenário                 | Permissões                                  |
|:------------------------------------|:---------------------------------------------|
| Chamando                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| Reuniões                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |
| Presença                 | Presence.Read, Presence.Read.All |
| Registros de chamadas             | CallRecords.Read.All |

## <a name="common-use-cases"></a>Casos de uso comuns

A tabela a seguir lista alguns dos usos comuns para a API de comunicações na nuvem.

| Casos de uso                         | Recursos REST                                 | Confira também  |
|:------------------------------------|:---------------------------------------------|:----------|
| Criando e associando chamadas 1-1 e de grupo   | [Call](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true&preserve-view=true)| [Métodos para chamadas](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true#methods&preserve-view=true)|
|Chamadas IVR   |     | [Métodos para IVR](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta?&preserve-view=true&preserve-view=true)
| Controles de chamada (participante) | [Participante](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true&preserve-view=true)   ||
|Reuniões|[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true)| [Métodos para reuniões](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true#methods&preserve-view=true)|
|Presença | [presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) | [Métodos para presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true#methods) |
| Recuperar registros de chamadas | [callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta&preserve-view=true&preserve-view=true) | [Assinaturas do Webhook](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true&preserve-view=true) |

## <a name="common-properties"></a>Propriedades comuns

| Recurso                | Propriedades                             |
|:------------------------------------|:---------------------------------------------|
| call                               | [propriedades de chamada](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true#properties&preserve-view=true)  |
| participante                         | [propriedades dos participantes](/graph/api/resources/participant?view=graph-rest-beta?view=graph-rest-v1.0&preserve-view=true#properties&preserve-view=true) |
| onlineMeeting                            | [Propriedades onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true#properties&preserve-view=true)                     |
| presença | [Propriedades de presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true#properties) |
| callRecord | [Propriedades do callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta&preserve-view=true#properties) |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="see-also"></a>Confira também

- [Exemplos da API de comunicações na nuvem](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [SDK de sinalização de comunicação](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [SDK de mídia de comunicação](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)


