---
title: Trabalhando com a API de comunicações no Microsoft Graph
description: A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como seus aplicativos e serviços podem interagir com os usuários, ativando os recursos de voz e vídeo.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: e6e6c4ba8d262ac01846b6ed06938b2c5c89350b
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581135"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a>Trabalhando com a API de comunicações no Microsoft Graph

A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como você ou sua organização podem interagir com outros usuários, habilitando os principais recursos e funções de comunicação de seus aplicativos e serviços. Você pode usar esta API para criar e receber chamadas, além de criar e recuperar coordenadas de reunião.

Você pode usar a API de comunicações para criar aplicativos de serviço (bots) que atuam como participantes de uma chamada e que criam e recuperam reuniões em nome dos usuários.
Essa API fornece funcionalidade de chamada, bem como a capacidade de criar e recuperar reuniões online. Você pode usar aplicativos de serviço (bots) com esta API, onde o bot pode atuar como participante de suas chamadas de VoIP ou reuniões do Microsoft Teams, por exemplo.

## <a name="authorization"></a>Autorização

É necessária uma das seguintes [permissões](/graph/permissions-reference#calls-permissions) para acessar a API de comunicações. Essas permissões precisam ser concedidas pelo administrador

| Cenário                 | Permissões                                  |
|:------------------------------------|:---------------------------------------------|
| Chamando                 | Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All |
| Reuniões                 | OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All |
| Registros de chamadas             | CallRecords.Read.All |
| Presenças             | Presence.Read, Presence.Read.All |

## <a name="common-use-cases"></a>Casos de uso comuns

A tabela a seguir lista alguns dos usos comuns para a API de comunicações.

| Casos de uso                         | Recursos REST                                 | Confira também  |
|:------------------------------------|:---------------------------------------------|:----------|
| Criando e associando chamadas 1-1 e de grupo   | [Call](/graph/api/resources/call?view=graph-rest-v1.0)| [Métodos para chamadas](/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|Chamadas IVR   |     | [Métodos para IVR](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| Controles de chamada (participante) | [Participante](/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|Reuniões|[onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [Métodos para reuniões](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|
| Recuperar registros de chamadas | [callRecord](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) | [Assinaturas do Webhook](/graph/api/resources/webhooks?view=graph-rest-1.0) |
|Presenças|[presença](/graph/api/resources/presence?view=graph-rest-v1.0)||

## <a name="common-properties"></a>Propriedades comuns

| Recurso                | Propriedades                             |
|:------------------------------------|:---------------------------------------------|
| call                               | [propriedades de chamada](/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| participante                         | [propriedades dos participantes](/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| onlineMeeting                            | [Propriedades onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |
| callRecord | [Propriedades do callRecord](/graph/api/resources/callrecords-callrecord#properties) |
|presença|[presença](/graph/api/resources/presence?view=graph-rest-v1.0)|

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="see-also"></a>Confira também

- [Exemplos da API de comunicações](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [SDK de sinalização de comunicação](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [SDK de mídia de comunicação](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)