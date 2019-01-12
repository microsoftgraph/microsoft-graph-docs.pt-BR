---
title: tipo de recurso de chamada
description: O recurso de **chamada** é criado quando há uma chamada de entrada para o aplicativo ou o aplicativo cria uma nova chamada de saída por meio de um `POST` em `app/calls`.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6c303ebe01e6051a29a932d9547f20293cb07a53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958555"
---
# <a name="call-resource-type"></a>tipo de recurso de chamada

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **chamada** é criado quando há uma chamada de entrada para o aplicativo ou o aplicativo cria uma nova chamada de saída por meio de um `POST` em `app/calls`.

Chamadas podem ser configuradas como uma ponto a ponto ou como uma chamada com vários participantes. Para criar ou ingressar em uma chamada com vários participantes, fornecer o `chatInfo` e `meetingInfo`. Se eles não são fornecidos, uma nova reunião ad-hoc é criada automaticamente. Para uma chamada de entrada, esses valores de registro em um repositório altamente disponível, para que seu aplicativo para reingressar a chamada no caso de falha de seu aplicativo.

Embora a mesma identidade não pode ser convidada várias vezes, é possível para um aplicativo para participar da reunião mesmo várias vezes. Cada vez que as associações de aplicativo, uma chamada distinta `id` é fornecido para a chamada para a reunião. Recomendamos que você use identidades separadas para ingressar na reunião para que os clientes para exibi-las como diferentes participantes.

## <a name="methods"></a>Métodos

| Método                                                            | Tipo de retorno                                       | Descrição                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Fazer chamada](../api/call-get.md)                                    | [chamada](call.md)                                   | Leia as propriedades do objeto **de chamada** .      |
| [Delete](../api/call-delete.md)                                   |                                                   | Excluir ou desligamento uma **chamada**de ativo.        |
| **Tratamento de chamada**                                                 |                                                   |                                              |
| [Resposta](../api/call-answer.md)                                   |                                                   | Atenda uma chamada de entrada.                     |
| [Reject](../api/call-reject.md)                                   |                                                   | Rejeite uma chamada de entrada.                     |
| [Redirecionar](../api/call-redirect.md)                               |                                                   | Redirecione uma chamada recebida.                   |
| [Transferir](../api/call-transfer.md)                               |                                                   | Transferir uma chamada                              |
| **Com vários participantes**                                                   |                                                   |                                              |
| [Participantes da lista](../api/call-list-participants.md)             | coleção de [participante](participant.md)          | Obtenha uma coleção de objetos dos participantes.         |
| [Convidar participantes](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | Convide participantes à chamada ativa.      |
| [Ativar Mudo de todos os participantes](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | Ativar Mudo de todos os participantes na chamada.           |
| [Configurar Mixer de áudio](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | Configure áudio na conversa com vários participantes.  |
| [Criar audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | Crie um novo audioRoutingGroup pelo lançamento à coleção audioRoutingGroups. |
| [Lista audioRoutingGroups](../api/call-list-audioroutinggroups.md) | coleção [audioRoutingGroup](audioroutinggroup.md)|Obtenha uma coleção de objetos audioRoutingGroup.  |
| **Resposta interativa de voz**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | Reproduza um prompt na chamada.                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | Registre a chamada.                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | Cancele o processamento de mídia.                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | Assine os tons DTMF.                     |
| **Operações de participante Self**                                   |                                                   |                                              |
| [Sem áudio](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | Ativar Mudo self na chamada.                       |
| [Desativar Mudo](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | Desativar o mudo self na chamada.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | Atualize os metadados para self na lista de participação.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | Iniciar e parar o compartilhamento de tela na chamada                                             |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                                                                   | Descrição                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | Coleção de cadeia de caracteres                                                                                      | A lista de modalidades ativas. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`. Somente leitura. Servidor foi gerado.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | O participante que atendeu a chamada. Somente leitura. Servidor foi gerado.                                                                                                                                |
| callRoutes          | coleção [callRoute](callroute.md)                                                                   | As informações de roteamento em como a chamada foi redirecionada. Somente leitura. Servidor foi gerado.                                                                                                                |
| callbackUri         | String                                                                                                 | A ID de inscrição ou de retorno de chamada no qual serão entregues retornos de chamada.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | As informações de bate-papo.                                                                                                                                                                               |
| direção           | String                                                                                                 | A direção da chamada. Os valores possíveis são `incoming` ou `outgoing`. Somente leitura. Servidor foi gerado.                                                                                            |
| id                  | String                                                                                                 | Somente leitura. Servidor foi gerado.                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) ou [serviceHostedMediaConfig](servicehostedmediaconfig.md) | A configuração de mídia.                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Contém os recursos de uma reunião.                                                                                                                                                             |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) ou [tokenMeetingInfo](tokenmeetinginfo.md)             | As informações da reunião.                                                                                                                                                                            |
| myParticipantId     | String                                                                                                 | Somente leitura. Servidor foi gerado.                                                                                                                                                                        |
| requestedModalities | String collection                                                                                      | A lista de modalidades solicitadas. | Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | As informações de resultado. Por exemplo, pode conter motivo de encerramento. Somente leitura. Servidor foi gerado.                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | Tempo limite de toque para chamadas ponto a ponto                                                                                                                                                     |
| routingPolicies     | String collection                                                                                      | Os valores possíveis são: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`.                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | O autor da chamada.                                                                                                                                                                         |
| estado               | String                                                                                                 | O estado de chamada. Os valores possíveis são: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Somente leitura. Servidor foi gerado.                         |
| subject             | String                                                                                                 | O assunto da conversa.                                                                                                                                                                    |
| destinos             | coleção [participantInfo](participantinfo.md)                                                       | As metas da chamada.                                                                                                                                                                            |
| tenantId            | String                                                                                                 | tenantId no Windows Azure Active Directory.                                                                                                                                                                 |
| terminationReason   | String                                                                                                 | Somente leitura. Servidor foi gerado.                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Somente leitura. Servidor foi gerado.                                                                                                                                                                        |

> Observação: Propriedades marcadas como `Server generated` serão ignorados durante o processamento `POST` em `app/calls`.

## <a name="relationships"></a>Relações

| Relação        | Tipo                                                 | Descrição                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | coleção [audioRoutingGroup](audioroutinggroup.md) | Somente leitura. Anulável.                                                |
| operations          | coleção [commsOperation](commsoperation.md)       | Somente leitura. Anulável.                                                |
| participantes        | coleção de [participante](participant.md)             | Somente leitura. Anulável.                                                |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "activeModalities",
    "answeredBy",
    "callRoutes",
    "chatInfo",
    "direction",
    "id",
    "meetingCapability",
    "meetingInfo",
    "myParticipantId",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "activeModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "answeredBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "#microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

> **Observação:** Você encontrará URL de ingresso de uma reunião agendada com Microsoft Teams. Aqui está como extrair os dados da URL e o preenchimento `chatInfo` e `meetingInfo`.

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call",
  truncated: true
}-->
```json
{
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "id": "4b444206-207c-42f8-92a6-e332b41c88a2"
      }
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
