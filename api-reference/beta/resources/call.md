---
title: Tipo de recurso de chamada
description: O recurso **call** é criado quando há uma chamada recebida para o aplicativo ou quando o aplicativo cria uma nova chamada realizada por meio de um `POST` em `app/calls`.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a7eb47d65d07cbdb88712a3b71b7de24b7d366cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572959"
---
# <a name="call-resource-type"></a>Tipo de recurso de chamada

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **call** é criado quando há uma chamada recebida para o aplicativo ou quando o aplicativo cria uma nova chamada realizada por meio de um `POST` em `app/calls`.

As chamadas podem ser configuradas como uma chamada ponto a ponto ou com vários participantes. Para criar ou ingressar em uma chamada com vários participantes, forneça `chatInfo` e `meetingInfo`. Caso não sejam fornecidos, uma nova reunião ad hoc é criada automaticamente. Para uma chamada recebida, grave esses valores em um armazenamento altamente disponível para que o aplicativo reingresse na chamada caso enfrente uma falha.

Embora a mesma identidade não possa ser convidada várias vezes, é possível que um aplicativo ingresse na mesma reunião várias vezes. Toda vez que o aplicativo ingressa, uma chamada distinta `id` é fornecida para essa chamada à reunião. É recomendável usar identidades separadas para ingressar na reunião para que os clientes as exibam como participantes diferentes.

## <a name="methods"></a>Métodos

| Método                                                            | Tipo de retorno                                       | Descrição                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Get call](../api/call-get.md)                                    | [call](call.md)                                   | Leia propriedades do objeto **call**.      |
| [Delete](../api/call-delete.md)                                   |                                                   | Exclua ou desligue uma **chamada** ativa.        |
| **Tratamento de chamadas**                                                 |                                                   |                                              |
| [Answer](../api/call-answer.md)                                   |                                                   | Atenda às chamadas recebidas.                     |
| [Reject](../api/call-reject.md)                                   |                                                   | Rejeite as chamadas recebidas.                     |
| [Redirect](../api/call-redirect.md)                               |                                                   | Redirecione as chamadas recebidas.                   |
| [Transfer](../api/call-transfer.md)                               |                                                   | Transfira uma chamada.                              |
| **Vários participantes**                                                   |                                                   |                                              |
| [List participants](../api/call-list-participants.md)             | [participant](participant.md) collection          | Obtenha uma coleção do objeto participant.         |
| [Invite Participants](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | Convide participantes para a chamada ativa.      |
| [Mute All Participants](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | Ative o mudo para todos os participantes na chamada.           |
| [Configure Audio Mixer](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | Configure áudio na conversa com vários participantes.  |
| [Create audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | Crie um novo audioRoutingGroup postando-o na coleção audioRoutingGroups. |
| [List audioRoutingGroups](../api/call-list-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md) collection|Obtenha uma coleção do objeto audioRoutingGroup.  |
| **Interactive-Voice-Response**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | Reproduza uma solicitação na chamada.                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | Registre a chamada.                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | Cancele o processamento de mídia.                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | Inscreva-se nos tons DTMF.                     |
| **Operações do próprio participante**                                   |                                                   |                                              |
| [Mute](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | Ative o mudo para si mesmo na chamada.                       |
| [Unmute](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | Desative o mudo para si mesmo na chamada.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | Atualize seus metadados na lista de participantes.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | Inicie e interrompa o compartilhamento de tela na chamada.                                             |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                                                                   | Descrição                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | coleção modality                                                                                      | A lista de modalidades ativas. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`. Somente leitura. Servidor gerado.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | O participante que atendeu a chamada. Somente leitura. Servidor gerado.                                                                                                                                |
| callRoutes          | [callRoute](callroute.md) collection                                                                   | As informações de roteamento sobre como a chamada foi redirecionada. Somente leitura. Servidor gerado.                                                                                                                |
| callbackUri         | String                                                                                                 | A ID de retorno de chamada ou de assinatura à qual os retornos serão entregues.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | As informações de chat.                                                                                                                                                                               |
| direção           | callDirection                                                                                          | A direção da chamada. Os valores possíveis são `incoming` ou `outgoing`. Somente leitura. Servidor gerado.                                                                                            |
| id                  | String                                                                                                 | Somente leitura. Servidor gerado.                                                                                                                                                                        |
| mediaConfig         | [mediaConfig](mediaconfig.md)                                                                          | A configuração de mídia.                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Contém os recursos de uma reunião.                                                                                                                                                             |
| meetingInfo         | [meetingInfo](meetinginfo.md)                                                                          | As informações da reunião.                                                                                                                                                                            |
| myParticipantId     | String                                                                                                 | Somente leitura. Servidor gerado.                                                                                                                                                                        |
| requestedModalities | coleção modality                                                                                      | A lista de modalidades solicitadas. | Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | As informações de resultado. Por exemplo pode incluir o motivo de término. Somente leitura. Servidor gerado.                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | Tempo limite do toque para chamadas realizadas de ponto a ponto                                                                                                                                                     |
| routingPolicies     | coleção routingPolicy                                                                                      | Os valores possíveis são: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`.                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | O remetente da chamada.                                                                                                                                                                         |
| state               | callState                                                                                                 | O estado da chamada. Os valores possíveis são: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Somente leitura. Servidor gerado.                         |
| subject             | String                                                                                                 | O assunto da conversa.                                                                                                                                                                    |
| targets             | [participantInfo](participantinfo.md) collection                                                       | O destinatário da chamada.                                                                                                                                                                            |
| tenantId            | String                                                                                                 | O tenantid no Azure Active Directory.                                                                                                                                                                 |
| terminationReason   | String                                                                                                 | Somente leitura. Servidor gerado.                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Somente leitura. Servidor gerado.                                                                                                                                                                        |

> Observação: propriedades marcadas como `Server generated` são ignoradas ao processar `POST` em `app/calls`.

## <a name="relationships"></a>Relações

| Relação        | Tipo                                                 | Descrição                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md) collection | Somente leitura. Anulável.                                                |
| operations          | [commsOperation](commsoperation.md) collection       | Somente leitura. Anulável.                                                |
| participants        | [participant](participant.md) collection             | Somente leitura. Anulável.                                                |

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
    "mediaConfig",
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
  "activeModalities": ["modality"],
  "answeredBy": {"@odata.type": "microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "direction": "callDirection",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["modality"],
  "resultInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["routingPolicy"],
  "source": {"@odata.type": "microsoft.graph.participantInfo"},
  "state": "callState",
  "subject": "String",
  "targets": [{"@odata.type": "microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "microsoft.graph.toneInfo"}
}
```

> **Observação:** você encontrará a URL de ingresso em uma reunião agendada com o Microsoft Teams. Veja aqui como extrair os dados da URL e preencher `chatInfo` e `meetingInfo`.

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call",
  "truncated": true
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
<!--
{
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/call.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
