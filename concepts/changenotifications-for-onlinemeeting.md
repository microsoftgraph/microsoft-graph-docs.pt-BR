---
title: Obter notificações de alteração para as atualizações de chamada de reunião no Microsoft Graph
description: As notificações de alteração no Microsoft Graph permitem que você assine chamadas iniciadas/encerradas e em atualizações de lista de participantes de chamadas para reuniões do Microsoft Teams.
author: benlee-msft
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: bca104717d5b6c50f53eabe21e450ea3520d2a8b
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63376515"
---
# <a name="get-change-notifications-for-meeting-call-updates-in-microsoft-graph"></a>Obter notificações de alteração para as atualizações de chamada de reunião no Microsoft Graph

As notificações de alteração no Microsoft Graph permitem que você assine chamadas iniciadas/encerradas e em atualizações de lista de participantes de chamadas para reuniões do Microsoft Teams. As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma assinatura. Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.

### <a name="subscribe-to-messages-across-all-channels"></a>Assine para receber mensagens em todos os canais

Para obter notificações de alteração em eventos de chamada de uma reunião em um aplicativo, assine `/communications/onlineMeetings/{meeting-id}`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

#### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All | beta |

#### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/communications/onlineMeetings/{meeting-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2021-02-01T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```
## <a name="notifications-with-encrypted-resource-data"></a>Notificações com dados de recursos criptografados
```json
{
  "value": [{
    "subscriptionId": "{Subscription id}",
    "clientState": "{secret client state}",
    "changeType": "updated",
    "tenantId": "{Organization/Tenant id}",
    "resource": "communications/onlineMeeting/{meeting-id}",
    "subscriptionExpirationDateTime": "2022-02-28T02:00:00-08:00",
    "resourceData": {
      "@odata.id": "communications/onlineMeetings/{meeting-id}",
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "communications/onlineMeetings/{meeting-id}"
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

Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).

A carga de notificação descriptografada parece com a seguinte.
```json
{
  "@odata.type":"#microsoft.graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings/{meeting-id}",
  "id":"communications/onlineMeetings/{meeting-id}",
  "eventType":"Microsoft.Communication.CallStarted",
  "eventDateTime":"2022-02-28T18:41:33.0553203Z",
  "state":"active"
}
```

Você pode optar por omitir a criptografia se não incluir a propriedade **includeResourceData** ou definir esse valor como `false` no corpo da solicitação de assinatura.
## <a name="event-notifications-types"></a>Tipos de notificações de eventos
Estes são os eventos de reunião com suporte:
- CallStarted – Ocorre quando uma chamada de reunião é iniciada.
- CallEnded – Ocorre quando uma chamada de reunião foi encerrada.
- CallRosterUpdate – Ocorre quando um participante ingressa ou sai de uma chamada.

Os eventos **CallRosterUpdate** incluirão duas propriedades adicionais, **activeParticipants@delta** e **activeParticipants@remove**, para representar os participantes ingressando/saindo da chamada da reunião na propriedade **resourceData**.

## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
- [Recurso de reunião online](/graph/api/resources/onlinemeeting.md)
