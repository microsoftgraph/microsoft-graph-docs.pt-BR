---
title: Tipo de recurso de chamada
description: O recurso **call** é criado quando há uma chamada recebida para o aplicativo ou quando o aplicativo cria uma nova chamada realizada por meio de um `POST` em `app/calls`.
author: VinodRavichandran
localization_priority: Priority
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 65e17466121dedef36c72a0091974e2a2329494c
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747994"
---
# <a name="call-resource-type"></a>Tipo de recurso de chamada

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **call** é criado quando há uma chamada recebida para o aplicativo ou quando o aplicativo cria uma nova chamada realizada por meio de um `POST` em `app/calls`.

As chamadas podem ser configuradas como uma chamada ponto a ponto ou com vários participantes. Para criar ou ingressar em uma chamada com vários participantes, forneça `chatInfo` e `meetingInfo`. Caso não sejam fornecidos, uma nova reunião ad hoc é criada automaticamente. Para uma chamada recebida, grave esses valores em um armazenamento altamente disponível para que o aplicativo reingresse na chamada caso enfrente uma falha.

Embora a mesma identidade não possa ser convidada várias vezes, é possível que um aplicativo ingresse na mesma reunião várias vezes. Toda vez que o aplicativo ingressa, uma chamada distinta `id` é fornecida para essa chamada à reunião. É recomendável usar identidades separadas para ingressar na reunião para que os clientes as exibam como participantes diferentes.

## <a name="methods"></a>Métodos

| Método                                                             | Tipo de retorno                                                 | Descrição                                                                     |
|:-------------------------------------------------------------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| [Get](../api/call-get.md)                                     | [call](call.md)                                             | Leia propriedades do objeto **call**.                                         |
| [Delete](../api/call-delete.md)                                    | Nenhum                                                            | Exclua ou desligue uma **chamada** ativa.                                           |
| **Tratamento de chamadas**                                                  |                                                        |                                                                                 |
| [Resposta](../api/call-answer.md)                                    | Nenhum                                                            | Atenda às chamadas recebidas.                                                        |
| [Reject](../api/call-reject.md)                                    | Nenhum                                                            | Rejeite as chamadas recebidas.                                                        |
| [Redirecionar](../api/call-redirect.md)                                | Nenhum                                                            | Redirecione as chamadas recebidas.                                                      |
| [Transfer](../api/call-transfer.md)                                | Nenhum                                                            | Transferir uma chamada                                                                 |
| **Chamadas em Grupo**                                                    |                                                             |                                                                                 |
| [List participants](../api/call-list-participants.md)              | [participant](participant.md) collection                    | Obtenha uma coleção do objeto participant.                                            |
| [Convidar participantes](../api/participant-invite.md)                | [commsOperation](commsoperation.md)                         | Convide participantes para a chamada ativa.                                         |
| [Ativar mudo para todos os participantes](../api/participant-muteall.md)             | [commsOperation](commsoperation.md)                         | Ative o mudo para todos os participantes em uma chamada.                                              |
| [Ativar mudo para participante](../api/participant-mute.md)                     | [muteParticipantOperation](muteparticipantoperation.md)     | Ative o mudo para participante na chamada de grupo.                                           |
| [Configurar o mixer de áudio](../api/participant-configuremixer.md)      | [commsOperation](commsoperation.md)                         | Configure áudio na conversa com vários participantes.                                     |
| [Create audioRoutingGroup](../api/call-post-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md)                   | Crie um novo audioRoutingGroup postando-o na coleção audioRoutingGroups. |
| [List audioRoutingGroups](../api/call-list-audioroutinggroups.md)  | [audioRoutingGroup](audioroutinggroup.md) collection        | Obtenha uma coleção do objeto audioRoutingGroup.                                      |
| **Interactive-Voice-Response**                                     |                                                             |                                                                                 |
| [PlayPrompt](../api/call-playprompt.md)                            | [playPromptOperation](playpromptoperation.md)               | Reproduza uma solicitação na chamada.                                                        |
| [Record](../api/call-record.md)                                    | [recordOperation](recordoperation.md)                       | Grave um clipe de áudio curto da chamada.                                        |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)      | [commsOperation](commsoperation.md)                         | Cancele o processamento de mídia.                                                        |
| [SubscribeToTone](../api/call-subscribetotone.md)                  | [commsOperation](commsoperation.md)                         | Inscreva-se nos tons DTMF.                                                        |
| **Operações do próprio participante**                                    |                                                             |                                                                                 |
| [Mute](../api/call-mute.md)                                        | [muteParticipantOperation](muteparticipantoperation.md)     | Ative o mudo para si mesmo na chamada.                                                          |
| [Unmute](../api/call-unmute.md)                                    | [unmuteParticipantOperation](unmuteparticipantoperation.md) | Desative o mudo automaticamente na chamada.                                                        |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md)  | Nenhum                                                            | Inicie e interrompa a tela de compartilhamento na chamada.                                      |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                                                                   | Descrição                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | String Collection                                                                                      | A lista de modalidades ativas. Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`. Somente leitura.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | O participante que atendeu a chamada. Somente leitura.                                                                                                                                |
| callRoutes          | [callRoute](callroute.md) collection                                                                   | As informações de roteamento sobre como a chamada foi redirecionada. Somente leitura.                                                                                                                |
| callbackUri         | String                                                                                                 | A URL de retorno de chamada à qual os retornos serão entregues. Deve ser `https`.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | As informações de chat. Informações necessárias para cenários de reunião.                                                                                                                                |
| direction           | String                                                                                                 | A direção da chamada. Os valores possíveis são `incoming` ou `outgoing`. Somente leitura.                                                                                            |
| id                  | String                                                                                                 | A ID de chamada. Somente leitura.                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) ou [serviceHostedMediaConfig](servicehostedmediaconfig.md) | A configuração de mídia. As informações necessárias para a criação de chamadas ponto a ponto ou para entrar em reuniões.                                                                        |
| mediaState          | [callMediaState](callmediastate.md)                                                                    | Somente leitura. O estado da mídia de chamadas. |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Contém os recursos de uma reunião. Somente leitura.                                                                                                       |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) ou [tokenMeetingInfo](tokenmeetinginfo.md)             | As informações da reunião. Informações necessárias para cenários de reunião.                                                                                                              |
| myParticipantId     | String                                                                                                 | Somente leitura.                                                                                                                                                                        |
| requestedModalities | String collection                                                                                      | A lista de modalidades solicitadas. | Os valores possíveis são: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | As informações de resultado. Por exemplo pode incluir o motivo de término. Somente leitura.                                                                                                        |
| ringingTimeoutInSeconds | Int32                                                                                              | Tempo limite do toque em segundos para chamadas realizadas de ponto a ponto. O valor máximo para esse atributo é de 115 segundos.                                                                                        |
| routingPolicies     | Coleção de cadeias de caracteres                                                                                      | Essa propriedade é aplicável somente às chamadas ponto a ponto. Os valores possíveis são: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`, `preferSkypeForBusiness`.                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | O remetente da chamada.                                                                                                                                                                         |
| state               | String                                                                                                 | O estado da chamada. Os valores possíveis são: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Somente leitura.                          |
| assunto             | String                                                                                                 | O assunto da conversa.                                                                                                                                                                    |
| targets             | [participantInfo](participantinfo.md) collection                                                       | O destinatário da chamada. Informações necessárias para criar chamadas ponto a ponto.                                                                                                            |
| tenantId            | String                                                                                                 | Somente leitura. `tenantId` em Azure Active Directory.                                                                                                                        |
| terminationReason   | String                                                                                                 | Somente leitura.                                                                                                                                                                       |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Somente leitura.                                                                                                                                                                        |

## <a name="relationships"></a>Relacionamento

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
    "mediaState",
    "meetingCapability",
    "meetingInfo",
    "myParticipantId",
    "replacesContext",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "source",
    "subject",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "keyProperty":"id",
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
  "mediaState": {"@odata.type": "#microsoft.graph.callMediaState"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "replacesContext": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding | preferSkypeForBusiness"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

> **Observação:** você encontrará a URL de ingresso em uma reunião agendada com o Microsoft Teams. Veja aqui como extrair os dados da URL e preencher `chatInfo` e `meetingInfo`.

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
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
