---
title: Alterar as notificações para os recursos do Microsoft Teams
description: Assine as alterações de recursos e dados de recursos no Microsoft Teams usando a API do Microsoft Graph. Saiba mais sobre tipos de notificação de alteração e cargas.
author: anandab-msft
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0091ded928de826220b837a66873e736fb1e84bc
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555566"
---
# <a name="change-notifications-for-microsoft-teams-resources"></a>Alterar as notificações para os recursos do Microsoft Teams

As notificações de alteração para recursos do Microsoft Teams Microsoft Graph permitem que você assine alterações (criar, atualizar e excluir) em um recurso. As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma [assinatura](/graph/api/resources/webhooks). Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.

> [!NOTE]
> O tempo máximo que uma assinatura pode durar é de 60 minutos; no entanto, as assinaturas podem ser renovadas até que o chamador tenha permissões para acessar o recurso.

## <a name="change-notification-types"></a>Tipoos de notificações de alteração

O Microsoft Teams dá suporte a dois tipos de notificações de alteração:

- **Alterar notificação para controlar todas as alterações relacionadas a um recurso no locatário:** Por exemplo, você pode assinar alterações em mensagens em qualquer canal no locatário e ser notificado sempre que uma mensagem for criada, atualizada ou excluída em qualquer canal no locatário. Essas notificações podem ter [Requisitos de licenciamento e pagamento](/graph/teams-licenses), como notificações de alteração para [mensagens](teams-changenotifications-chatmessage.md) e [assinatura](teams-changenotifications-chatMembership.md).

- **Alterar notificação para controlar todas as alterações de um recurso específico:** Por exemplo, você pode assinar alterações em mensagens em um canal específico e ser notificado sempre que uma mensagem for criada, atualizada ou excluída nesse canal.

Para obter detalhes sobre quais recursos dão suporte a quais tipos de notificações de alteração, consulte [Notificações de Alteração do Microsoft Graph](webhooks.md).

## <a name="supported-resources"></a>Recursos com suporte
A tabela a seguir lista os recursos do Microsoft Teams e os caminhos de recursos correspondentes com suporte no momento.

| **Recurso** | **Trajetórias dos recursos com suporte** | **Os dados do recurso podem ser incluídos nas notificações** |
|:----------------|:------------|:-----------------------------------------|
| [Canal](/graph/api/resources/channel) do Teams | Alterações nos canais em todas as equipes:<br>`/teams/getAllChannels` <br>Alterações no canal em uma equipe específica:<br>`/teams/{id}/channels` | Sim |
| [Chat](/graph/api/resources/chat) do Teams | Alterações em qualquer chat no locatário:<br>`/chats` <br>Alterações em um chat específico:<br>`/chats/{id}` | Sim |
| Teams [chatMessage](/graph/api/resources/chatMessage) | Alterações nas mensagens de chat em todos os canais de todas as equipes:<br>`/teams/getAllMessages` <br>Alterações nas mensagens de um chat específico:<br>`/teams/{id}/channels/{id}/messages`<br>Alterações nas mensagens de todos os chats:<br>`/chats/getAllMessages` <br>Alterações nas mensagens de um chat específico:<br>`/chats/{id}/messages`<br>Alterações nas mensagens de chat em todos os chats de que um usuário específico faz parte:<br>`/users/{id}/chats/getAllMessages` | Sim |
| [conversationMember](/graph/api/resources/conversationMember) do Teams | Alterações na associação em uma equipe específica:<br>`/teams/{id}/members` <br> Alterações na associação em um chat específico:<br>`/chats/{id}/members` <br> Alterações na associação em todos os chats:<br>`/chats/getAllMembers` <br> Alterações na associação em todos os canais em uma equipe específica:<br>`teams/{id}/channels/getAllMembers` | Sim |
| Equipe do [Teams](/graph/api/resources/team) | Alterações em qualquer equipe no locatário:<br>`/teams` <br>Alterações em uma equipe específica:<br>`/teams/{id}` | Sim |
 

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

A carga de notificação descriptografada parece com a seguinte. A carga descriptografada para o exemplo anterior está em conformidade com o esquema [chatMessage](/graph/api/resources/chatMessage). A carga é semelhante à devolvida pelas operações GET.

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

> [!NOTE]
> As chamadas GET sempre retornarão o estado atual do recurso. Se o recurso for alterado entre quando a notificação for enviada e quando o recurso for recuperado, a operação retornará o recurso atualizado.

## <a name="see-also"></a>Confira também

- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
