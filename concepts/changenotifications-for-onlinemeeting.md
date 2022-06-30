---
title: Obter notificações de alteração para as atualizações de chamada de reunião no Microsoft Teams
description: Use as notificações de alteração no Microsoft Graph para permitir que você assine chamadas iniciadas/encerradas e em atualizações de lista de participantes de chamadas para reuniões online do Microsoft Teams.
author: benlee-msft
ms.localizationpriority: high
ms.prod: cloud-communications
ms.custom: scenarios:getting-started
ms.openlocfilehash: fd3fcde6679729f44931f2d9564bc2c62d7b169e
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556203"
---
# <a name="get-change-notifications-for-microsoft-teams-meeting-call-updates"></a>Obter notificações de alteração para as atualizações de chamada de reunião no Microsoft Teams

Altere as notificações no Microsoft Graph para permitir que você assine chamadas iniciadas/encerradas e em atualizações de lista de participantes de chamadas para reuniões online do Microsoft Teams. As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma assinatura. Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.

## <a name="subscribe-to-messages-across-all-channels"></a>Assine para receber mensagens em todos os canais

Para obter notificações de alteração em eventos de chamada de uma reunião em um aplicativo, assine `/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'`. Este recurso oferece suporte a [ incluindo dados de recursos ](/graph/webhooks-with-resource-data) na notificação.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All | beta |

### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2021-02-01T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="joinweburl"></a>JoinWebUrl

A URL de ingresso para a reunião está incluída na propriedade joinWebUrl do recurso [onlineMeeting](/graph/api/resources/onlineMeeting) ou no cliente do Teams para uma reunião.

## <a name="notifications-with-encrypted-resource-data"></a>Notificações com dados de recursos criptografados

```json
{
  "value": [{
    "subscriptionId": "{Subscription id}",
    "clientState": "{secret client state}",
    "changeType": "updated",
    "tenantId": "{Organization/Tenant id}",
    "resource": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
    "subscriptionExpirationDateTime": "2022-02-28T00:00:00.0000000Z",
    "resourceData": {
      "@odata.id": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'"
    },
    "organizationId": "{Organization/Tenant id}",
    "encryptedContent": {
      "data": "{Encrypted content}",
      "dataSignature": "{Encrypted data signature}",
      "dataKey": "{Encrypted data key for encrypting content}",
      "encryptionCertificateId": "{User specified id of encryption certificate}",
      "encryptionCertificateThumbprint": "{Encrpytion certification thumbprint}"
    }
  }],
  "validationTokens": ["{Validation Tokens}"]
}
```

Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](/graph/webhooks-with-resource-data).

## <a name="event-notifications-types"></a>Tipos de notificações de eventos

Estes são os eventos de reunião com suporte:
- CallStarted – Ocorre quando uma chamada de reunião é iniciada.
- CallEnded – Ocorre quando uma chamada de reunião foi encerrada.
- CallRosterUpdate – Ocorre quando um participante ingressa ou sai de uma chamada.

### <a name="decrypted-payload-examples"></a>Exemplos de conteúdo descriptografado

#### <a name="callstartedcallended"></a>CallStarted/CallEnded

```json
{
  "@odata.type":"#Microsoft.Graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "eventType":"{Microsoft.Communication.CallStarted or Microsoft.Communication.CallEnded}",
  "eventDateTime":"2022-02-28T00:00:00.0000000Z",
  "state":"active"
}
```

#### <a name="callrosterupdate"></a>CallRosterUpdate

```json
{
  "@odata.type":"#Microsoft.Graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "eventType":"Microsoft.Communication.CallRosterUpdate",
  "eventDateTime":"2022-02-28T00:00:00.0000000Z",
  "state":"active",
  "activeParticipants@delta": ["{meetingParticipantInfo list of users that joined}"],
  "activeParticipants@remove": ["{meetingParticipantInfo list of users that left}"]
}
```

**Os eventos CallRosterUpdate** incluem duas propriedades adicionais, **activeParticipants@delta** para representar os participantes adicionados a uma reunião e **activeParticipants@remove** para participantes que saem da reunião online. Para obter mais informações sobre os participantes, consulte [o tipo de recurso meetingParticipantInfo](/graph/api/resources/meetingparticipants).

Você pode optar por omitir a criptografia se não incluir a propriedade **includeResourceData** ou definir esse valor como `false` no corpo da solicitação de assinatura. Isso adiciona as propriedades que teriam sido parte da carga criptografada para **resourcedata**.

## <a name="see-also"></a>Confira também

- [Notificações de alteração do Microsoft Graph](/graph/webhooks)
- [Visão geral da API do Microsoft Teams](/graph/teams-concept-overview)
- [Recurso de reunião online](/graph/api/resources/onlineMeeting)
