---
title: Tipo de recurso de chamada
description: O recurso **call** é criado quando há uma chamada recebida para o aplicativo ou quando o aplicativo cria uma nova chamada realizada por meio de um `POST` em `app/calls`.
author: ananmishr
localization_priority: Priority
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0764a7a4e5ca7845033f5f31a440ec183528da4d
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962314"
---
# <a name="call-resource-type"></a>Tipo de recurso de chamada

Namespace: microsoft.graph

O recurso **call** é criado quando há uma chamada recebida para o aplicativo ou quando o aplicativo cria uma nova chamada realizada por meio de um `POST` em `app/calls`.

As chamadas podem ser configuradas como uma chamada ponto a ponto ou de grupo. Para criar ou ingressar em uma chamada de grupo, forneça `chatInfo` e `meetingInfo`. Caso não sejam fornecidos, uma nova chamada de grupo é criada automaticamente. Para uma chamada recebida, grave esses valores em um armazenamento altamente disponível para que o aplicativo reingresse na chamada caso enfrente uma falha.

Embora a mesma identidade não possa ser convidada várias vezes, é possível que um aplicativo ingresse na mesma reunião várias vezes. Sempre que o aplicativo quiser ingressar, uma identidade separada deve ser fornecida para que os clientes possam exibi-las como diferentes.

> ** Observação: ** você poderá obter a URL de ingresso em uma reunião agendada com o Microsoft Teams. Extraia os dados da URL conforme mostrado para preencher `chatInfo` e `meetingInfo`.
```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
```
Se tornará:
```
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

## <a name="methods"></a>Methods

| Método                                                             | Tipo de retorno                                                 | Descrição                                                                     |
|:-------------------------------------------------------------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| [Get](../api/call-get.md)                                     | [call](call.md)                                             | Leia propriedades do objeto **call**.                                         |
| [Delete](../api/call-delete.md)                                    | Nenhum                                                            | Exclua ou desligue uma **chamada** ativa.                                           |
| [KeepAlive](../api/call-keepalive.md)                             | Nenhum                                                  | Certifique-se de que a chamada permanece ativa.
| **Tratamento de chamadas**                                                  |                                                        |                                                                                 |
| [Resposta](../api/call-answer.md)                                    | Nenhum                                                            | Atenda às chamadas recebidas.                                                        |
| [Reject](../api/call-reject.md)                                    | Nenhum                                                            | Rejeite as chamadas recebidas.                                                        |
| [Redirecionar](../api/call-redirect.md)                                | Nenhum                                                            | Redirecione as chamadas recebidas.                                                      |
| [Transfer](../api/call-transfer.md)                                | Nenhum                                                            | Transferir uma chamada                                                                 |
| **Chamadas em Grupo**                                                    |                                                             |                                                                                 |
| [List participants](../api/call-list-participants.md)              | [participant](participant.md) collection                    | Obtenha uma coleção do objeto participant.                                            |
| [Convidar participantes](../api/participant-invite.md)                | [commsOperation](commsoperation.md)                         | Convide participantes para a chamada ativa.                                         |
| [Ativar mudo para participante](../api/participant-mute.md)                     | [muteParticipantOperation](muteparticipantoperation.md)     | Ative o mudo para participante na chamada de grupo.                                           |
| **Interactive-Voice-Response**                                     |                                                             |                                                                                 |
| [PlayPrompt](../api/call-playprompt.md)                            | [playPromptOperation](playpromptoperation.md)               | Reproduza uma solicitação na chamada.                                                        |
| [RecordResponse](../api/call-record.md)                            | [recordOperation](recordoperation.md)                       | Registra uma resposta de áudio curta do chamador.                                        |
| [SubscribeToTone](../api/call-subscribetotone.md)                  | [commsOperation](commsoperation.md)                         | Inscreva-se nos tons DTMF.                                                        |
| **Operações do próprio participante**                                    |                                                             |                                                                                 |
| [Mute](../api/call-mute.md)                                        | [muteParticipantOperation](muteparticipantoperation.md)     | Ative o mudo para si mesmo na chamada.                                                          |
| [Unmute](../api/call-unmute.md)                                    | [unmuteParticipantOperation](unmuteparticipantoperation.md) | Desative o mudo automaticamente na chamada.                                                        |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md)  | Nenhum                                                        | Inicie e interrompa a tela de compartilhamento na chamada.                                      |
| **Operações de gravação**                                           |                                                             |                                              |
| [UpdateRecordingStatus](../api/call-updaterecordingstatus.md)      | [updateRecordingStatusOperation](updateRecordingStatusOperation.md)               | Atualiza o status da gravação.                      |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                                                                   | Descrição                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| callbackUri         | String                                                                                                 | A URL de retorno de chamada à qual os retornos serão entregues. Deve ser `https`.                                                                                                                               |
| callRoutes         | [callRoute](callRoute.md) collection                                                                                                 | As informações de roteamento sobre como a chamada foi redirecionada. Apenas leitura.                                                                                                                |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | As informações de chat. Informações necessárias para ingressar em uma reunião.                                                                                                                              |
| direction           | String                                                                                                 | A direção da chamada. Os valores possíveis são `incoming` ou `outgoing`. Somente leitura.                                                                                            |
| id                  | String                                                                                                 | A ID de chamada. Somente leitura.                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) ou [serviceHostedMediaConfig](servicehostedmediaconfig.md) | A configuração de mídia. Obrigatório.                                                                        |
| mediaState          | [callMediaState](callmediastate.md)                                                                    | Somente leitura. O estado da mídia de chamadas. |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) ou [tokenMeetingInfo](tokenmeetinginfo.md)             | As informações de reunião necessárias para ingressar em uma reunião.                                                                                                            |
| myParticipantId     | String                                                                                                 | Somente leitura.                                                                                                                                                                        |
| requestedModalities | String collection                                                                                      | A lista de modalidades solicitadas. | Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | As informações de resultado. Por exemplo pode incluir o motivo de término. Somente leitura.                                                                                                        |
| source              | [participantInfo](participantinfo.md)                                                                  | O remetente da chamada.                                                                                                                                                                         |
| state               | String                                                                                                 | O estado da chamada. Os valores possíveis são: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Somente leitura.                          |
| assunto             | String                                                                                                 | O assunto da conversa.                                                                                                                                                                    |
| targets             | conjunto [invitationParticipantInfo](participantinfo.md)                                             | O destinatário da chamada. Informações necessárias para criar chamadas ponto a ponto.                                                                                                            |
toneInfo            | [toneInfo](toneinfo.md)                                                                                | Apenas leitura.                                                                                                                                                                        |
incomingContext            | [incomingContext](incomingContext.md)                                                                                | O contexto associado a uma chamada recebida.                                                                                                                                                                       |

## <a name="relationships"></a>Relações

| Relação        | Tipo                                                 | Descrição                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| operations          | [commsOperation](commsoperation.md) collection       | Somente leitura. Anulável.                                                |
| participants        | [participant](participant.md) collection             | Somente leitura. Anulável.                                                |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatInfo",
    "direction",
    "id",
    "incomingContext",
    "mediaState",
    "meetingInfo",
    "myParticipantId",
    "replacesContext",
    "resultInfo",
    "state",
    "source",
    "subject",
    "targets",
    "toneInfo"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "mediaState": {"@odata.type": "#microsoft.graph.callMediaState"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "replacesContext": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
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
  "suppressions": []
}
-->
