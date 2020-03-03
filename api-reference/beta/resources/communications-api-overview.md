---
title: Trabalhando com a API de comunicações no Microsoft Graph
description: A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como seus aplicativos e serviços podem interagir com os usuários, ativando os recursos de voz e vídeo.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 7869ac59f84f266542254fd0c8fc8ea97ee4815d
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394579"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a>Trabalhando com a API de comunicações no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como você ou sua organização podem interagir com outros usuários, habilitando os principais recursos e funções de comunicação de seus aplicativos e serviços. Você pode usar esta API para criar e receber chamadas, criar e recuperar coordenadas da reunião e verificar a presença dos usuários.

Você pode usar a API de comunicações para criar aplicativos de serviço (bots) que atuam como participantes de uma chamada e que criam e recuperam reuniões em nome dos usuários e verificar a disponibilidade e a atividade de presença.
Essa API fornece funcionalidade de chamada, bem como a capacidade de criar e recuperar reuniões online. Você pode usar aplicativos de serviço (bots) com esta API, onde o bot pode atuar como participante de suas chamadas de VoIP ou reuniões do Microsoft Teams, por exemplo.

## <a name="authorization"></a>Autorização

É necessária uma das seguintes [permissões](/graph/permissions-reference#calls-permissions) para acessar a API de comunicações. Essas permissões precisam ser concedidas pelo administrador

| Cenário                 | Permissões                                  |
|:------------------------------------|:---------------------------------------------|
| Chamando                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| Reuniões                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |
| Presença                 | Presence.Read, Presence.Read.All |
| Registros de chamadas             | CallRecords.Read.All |

## <a name="common-use-cases"></a>Casos de uso comuns

A tabela a seguir lista alguns dos usos comuns para a API de comunicações.

| Casos de uso                         | Recursos REST                                 | Confira também  |
|:------------------------------------|:---------------------------------------------|:----------|
| Criando e associando chamadas 1-1 e de grupo   | [Call](/graph/api/resources/call?view=graph-rest-beta)| [Métodos para chamadas](/graph/api/resources/call?view=graph-rest-beta#methods)|
|Chamadas IVR   |     | [Métodos para IVR](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| Controles de chamada (participante) | [Participante](/graph/api/resources/participant?view=graph-rest-beta)   ||
|Reuniões|[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [Métodos para reuniões](/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|
|Presença | [presença](/graph/api/resources/presence) | [Métodos para presença](/graph/api/resources/presence#methods) |
| Recuperar registros de chamadas | [callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) | [Assinaturas do Webhook](/graph/api/resources/webhooks?view=graph-rest-beta) |

## <a name="common-properties"></a>Propriedades comuns

| Recurso                | Propriedades                             |
|:------------------------------------|:---------------------------------------------|
| call                               | [propriedades de chamada](/graph/api/resources/call?view=graph-rest-beta#properties)  |
| participante                         | [propriedades dos participantes](/graph/api/resources/participant?view=graph-rest-beta#properties) |
| onlineMeeting                            | [Propriedades onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |
| presença | [Propriedades de presença](/graph/api/resources/presence#properties) |
| callRecord | [Propriedades do callRecord](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="see-also"></a>Confira também

- [Exemplos da API de comunicações](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [SDK de sinalização de comunicação](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [SDK de mídia de comunicação](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
