---
title: Obter notificações de alteração para qualquer alteração na associação do Teams usando o Microsoft Graph
description: Obter notificações de alteração para quaisquer alterações (criar, atualizar e excluir) na associação do Teams usando o Microsoft Graph
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 8d136e81c51ee470577706f1515f5950abdd58c641a30f340a62f1f9298626e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165501"
---
# <a name="get-change-notifications-for-changes-in-teams-membership-using-microsoft-graph"></a>Obter notificações de alteração para alterações na associação do Teams usando o Microsoft Graph

As notificações de alteração permitem que você se inscreva para receber alterações (criar, atualizar e excluir) na associação do Teams. Você pode ser notificado sempre que um membro for adicionado, removido ou atualizado em uma equipe. Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.

## <a name="subscribe-to-changes-in-membership-of-a-particular-team"></a>Inscrever-se para receber alterações na associação de uma equipe específica

Para obter notificações de alterações para alterações de membros em uma equipe específica, inscreva-se em `/teams/{team-id}/members`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

#### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | TeamMember.Read.All, TeamMember.ReadWrite.All | beta |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | TeamMember.Read.Group*, TeamMember.Read.All, TeamMember.ReadWrite.All   | beta |

>**Nota:** As permissões marcadas com * são suportadas como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

#### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
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

As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter o conteúdo para a mensagem. As chamadas GET sempre retornarão o estado atual da mensagem. Se a mensagem for alterada entre quando a notificação for enviada e quando a mensagem for recuperada, a operação retornará a mensagem atualizada.

## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)