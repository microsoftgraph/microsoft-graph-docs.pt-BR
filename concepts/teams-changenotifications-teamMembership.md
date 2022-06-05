---
title: Receba notificações de alteração de membros em equipes e canais usando o Microsoft Graph
description: Obtenha notificações de qualquer alteração (criar, atualizar e excluir) em equipes e canais de filiação usando o Microsoft Graph.
author: anandab
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: bdc228637496774dd7eb90dcd9b09dff8a6c9da7
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900472"
---
# <a name="get-change-notifications-for-membership-changes-in-teams-and-channels-using-microsoft-graph"></a>Receba notificações de alteração de membros em equipes e canais usando o Microsoft Graph

As notificações de alteração permitem que você assine as alterações de membros (criar, atualizar e excluir) em equipes e canais privados. Você pode ser notificado sempre que um membro é adicionado, removido ou atualizado em uma equipe ou em um canal privado. Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.

## <a name="subscribe-to-changes-in-membership-of-a-particular-team"></a>Inscrever-se para receber alterações na associação de uma equipe específica

Para obter notificações de alterações para alterações de membros em uma equipe específica, inscreva-se em `/teams/{team-id}/members`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | TeamMember.Read.All, TeamMember.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamMember.Read.Group*, TeamMember.Read.All, TeamMember.ReadWrite.All   |

>**Nota:** As permissões marcadas com * são suportadas como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-membership-changes-in-all-private-channels-of-a-particular-team"></a>Assinar as alterações de membros em todos os canais privados de uma determinada equipe

Para obter notificações de alteração de membros em todos os canais privados de uma determinada equipe, inscreva-se em `/teams/{team-id}/channels/getAllMembers`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

[!INCLUDE [teams-model-A-and-B-disclaimer](../includes/teams-model-A-and-B-disclaimer.md)]

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelMember.Read.All   |


### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/getAllMembers",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```




### <a name="notifications-with-resource-data"></a>Notificações com dados de recursos

Para notificações com dados de recursos, a carga se parece com a seguinte. Essa carga útil é para uma alteração de associação em uma equipe.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
        "resourceData": {
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
            "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
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

A carga útil para os eventos de adesão ao canal é semelhante à carga útil anterior, exceto que o **recurso** propriedade aponta para um membro do canal em vez de um membro da equipe.

Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).

A carga de notificação descriptografada parece com a seguinte. O conteúdo está em conformidade com o esquema [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true). A carga é semelhante à devolvida pelas operações GET.

```json
{
  "id": "/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [
    "owner"
  ],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="notifications-without-resource-data"></a>Notificações sem dados de recursos

Notificações sem dados de recursos dão informações suficientes para fazer chamadas GET para obter o conteúdo da mensagem. As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).

Para notificações sem dados de recursos, a carga se parecerá com o seguinte. Essa carga útil é para uma alteração de associação em uma equipe.

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
  "resourceData": {
    "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk",
    "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
    "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
  }
}
```

A carga útil para os eventos de adesão ao canal é semelhante à carga útil anterior, exceto que o **recurso** propriedade aponta para um membro do canal em vez de um membro da equipe.

As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter o conteúdo para a mensagem. As chamadas GET sempre retornarão o estado atual da mensagem. Se a mensagem for alterada entre quando a notificação for enviada e quando a mensagem for recuperada, a operação retornará a mensagem atualizada.

## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
