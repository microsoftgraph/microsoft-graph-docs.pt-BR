---
title: Obter notificações de alteração para equipes e canais usando o Microsoft Graph
description: Saiba como obter notificações de alterações (criar, atualizar e excluir) para equipes e canais usando as APIs do Microsoft Graph.
author: anandab
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 08a6b996d3ddbe721775a888b161e14788a485a9
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507763"
---
# <a name="get-change-notifications-for-teams-and-channels-using-microsoft-graph"></a>Obter notificações de alteração para equipes e canais usando o Microsoft Graph

As notificações de alteração permitem que você se inscreva para alterações (criar, atualizar e excluir) de equipes e canais. Você será notificado sempre que uma equipe ou canal for criado, atualizado ou excluído. Você também receberá os dados de recursos nas notificações e, portanto, evitará chamar a API para obter a carga útil.

## <a name="subscribe-to-changes-in-any-team-at-tenant-level"></a>Inscrever-se para alterações em qualquer equipe no nível de locatário

Para obter notificações de alteração para todas as alterações (criar, atualizar e excluir) relacionadas a qualquer equipe de um locatário, inscreva-se em `/teams`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All   | beta|

### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-team"></a>Inscrever-se para alterações em uma equipe em particular


Para obter notificações de alteração para todas as alterações relacionadas a uma equipe em particular de um locatário, inscreva-se em `/teams/{team-id}`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All | beta |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All    | beta |

>**Nota:** As permissões marcadas com * são suportadas como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


## <a name="subscribe-to-changes-in-any-channel-at-tenant-level"></a>Inscrever-se para alterações em qualquer canal no nível de locatário

Para obter notificações de alteração para todas as alterações (criar, atualizar e excluir) relacionadas a qualquer canal de um locatário, inscreva-se em `/teams/getAllChannels`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.


### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All | beta |

### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllChannels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-any-channel-of-a-particular-team"></a>Inscrever-se para alterações em qualquer canal em particular


Para obter notificações de alteração para todas as alterações relacionadas a qualquer canal em particular, inscreva-se em `/teams/{team-id}/channels`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação. Notificações de alteração para canais privados não são suportadas no contexto de delegação. Neste caso, um assinante deste recurso em contexto delegado receberá notificações somente para canais padrão sob uma equipe específica, não para canais privados.


### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All | beta |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All   | beta |

>**Nota:** As permissões marcadas com * são suportadas como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a>Notificações com dados de recursos

Para notificações com dados de recursos, a carga se parece com a seguinte. Essa carga é para uma alteração de propriedade em uma equipe.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.Team",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')"
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



A carga de notificação descriptografada parece com o seguinte. A carga está de acordo com o esquema de [equipes](/graph/api/resources/team?preserve-view=true). A carga é semelhante à devolvida pelas operações GET.

>**Observação:** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) não são expostos em dados de carga.

```json
{
  "id": "4c533ad3-e1dd-4277-a672-92ab64ed225c",
  "createdDateTime": "2021-03-18T10:31:14.597Z",
  "displayName": "Sample name",
  "description": "Sample description",
  "internalId": "19:2077546f765a42c1ba71236f4df70aa2@thread.tacv2",
  "specialization": "none",
  "visibility": "public",
  "webUrl": "https://teams.microsoft.com/l/team/19:2077546f724a42c1ba71236f4df79aa2%40thread.tacv2/conversations?groupId=4c533ad3-e1dd-4277-a672-92ab64ed225c&tenantId=0f2e8f59-862a-483b-9ca8-82a10665e17d",
  "isArchived": false,
  "isMembershipLimitedToOwners": false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowCreatePrivateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "allowCreateUpdateChannels": false,
    "allowDeleteChannels": false
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "moderate",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```


Para notificações com dados de recursos, a carga se parece com o seguinte. Esta carga é para uma alteração de propriedade em um canal.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')",
        "resourceData": {
            "id": "19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2",
            "@odata.type": "#Microsoft.Graph.Channel",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')"
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
  

A carga de notificação descriptografada parece com o seguinte. A carga está de acordo com o esquema de [canais](/graph/api/resources/channel?preserve-view=true). A carga é semelhante à devolvida pelas operações GET.

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


### <a name="notifications-without-resource-data"></a>Notificações sem dados de recursos

Notificações sem dados de recursos dão informações suficientes para fazer chamadas GET para obter o conteúdo da mensagem. As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).

Para notificações sem dados de recursos, a carga se parecerá com o seguinte. Essa carga é para uma alteração de propriedade em uma equipe.

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.Teams",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')"
  }
}
```

As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter o conteúdo para a mensagem. As chamadas GET sempre retornarão o estado atual da mensagem. Se a mensagem for alterada entre quando a notificação for enviada e quando a mensagem for recuperada, a operação retornará a mensagem atualizada.


>**Observação:** o endereço de email do canal não retorna na carga.

Para notificações sem dados de recursos, a carga se parecerá com o seguinte. Essa carga é para uma alteração de propriedade em uma equipe.

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
