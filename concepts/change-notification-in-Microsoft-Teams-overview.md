---
title: Alterar notificações para os recursos do Microsoft Teams usando Microsoft Graph
description: Saiba como obter notificações de alterações (criar, atualizar e excluir) para recursos no Microsoft Teams usando as APIs do Microsoft Graph
author: anandab-msft
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9433a4c5ee000fa34e125440168b865f1bb16172
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941551"
---
# <a name="change-notifications-for-microsoft-teams-resources-using-microsoft-graph"></a>Alterar notificações para os recursos do Microsoft Teams usando Microsoft Graph

As notificações de alteração habilitam você a assinar para receber alterações (criar, atualizar e excluir) um recurso. As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma [assinatura](/graph/api/resources/webhooks?preserve-view=true). Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.

> **Observação:** o tempo máximo que uma assinatura pode durar é 60 minutos; entretanto, as assinaturas podem ser renovadas até que o chamador tenha permissão para acessar o recurso.

## <a name="change-notification-types"></a>Tipoos de notificações de alteração
O Microsoft Teams dá suporte a dois tipos de notificações de alteração:
- **Altere a notificação para controlar todas as alterações relacionadas a um recurso no locatário** – por exemplo, você pode assinar alterações em mensagens em qualquer canal no locatário e ser notificado sempre que uma mensagem for criada, atualizada ou excluída em qualquer canal no locatário.
- **Altere a notificação para controlar todas as alterações de um recurso específico** - por exemplo, você pode assinar alterações em mensagens em um canal específico e ser notificado sempre que uma mensagem for criada, atualizada ou excluída nesse canal.

Para obter detalhes sobre quais recursos dão suporte a quais tipos de notificações de alteração, consulte [Notificações de Alteração do Microsoft Graph](webhooks.md).
 

## <a name="notification-payloads"></a>Cargas de notificação

Dependendo da sua assinatura, você pode receber a notificação com dados de recursos ou sem ele. Assinar com dados de recursos permite que você receba a carga da mensagem junto com a notificação, o que remove a necessidade de ligar de volta e obter o conteúdo.

### <a name="notifications-with-resource-data"></a>Notificações com dados de recursos

Para notificações com dados de recursos, a carga se parece com a seguinte.  Essa carga é para uma notificação correspondente ao recurso de mensagem de chat. A notificação real inclui as propriedades **resource** e **resourceData**, que representam o recurso que disparou a notificação.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).

A carga de notificação descriptografada parece com a seguinte. A carga descriptografada para o exemplo anterior está em conformidade com o esquema [chatMessage](/graph/api/resources/chatMessage?preserve-view=true). A carga é semelhante à devolvida pelas operações GET.

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a>Notificações sem dados de recursos

Notificações sem dados de recurso fornecem informações suficientes para fazer chamadas GET para obter o recurso. As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).

A carga parece ser a seguinte. Este conteúdo é para uma mensagem enviada em um canal.

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",  
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```
O exemplo anterior acima mostra uma notificação que corresponde a um recurso de mensagem de chat. A notificação real inclui as propriedades **resource** e **resourceData**, que representam o recurso que disparou a notificação. As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter a carga do recurso.

> **Observe** As chamadas GET sempre retornarão o estado atual do recurso. Se o recurso for alterado entre quando a notificação for enviada e quando o recurso for recuperado, a operação retornará o recurso atualizado.

## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
