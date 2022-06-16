---
title: Obtenha mensagens do sistema para o Microsoft Teams usando as APIs do Microsoft Graph
description: Saiba como o Microsoft Teams gera mensagens do sistema para eventos usando as APIs do Microsoft Graph.
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: b6a953acbd906a56d87df211209c52c432b79fae
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118316"
---
# <a name="get-system-messages-for-microsoft-teams-using-microsoft-graph-apis"></a>Obtenha mensagens do sistema para o Microsoft Teams usando as APIs do Microsoft Graph

O Microsoft Teams gera mensagens do sistema para eventos, como membros adicionados a um chat, nome da equipe atualizado e descrição atualizada do canal. As mensagens do sistema permitem que o chamador tenha insights sobre os eventos que aconteceram em uma equipe, um canal ou um chat.


O Microsoft Graph expõe as mensagens do sistema como parte das operações GET de [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-v1.0&preserve-view=true) e [Alterar notificações para mensagens de chat e canal](teams-changenotifications-chatmessage.md).


As mensagens do sistema são apresentadas como objetos de [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-v1.0&preserve-view=true).
Neste caso, a propriedade **messageType** é definida como `systemEventMessage` e a propriedade **eventDetail** fornece os detalhes do evento.


## <a name="supported-get-operations"></a>Suporta operações GET

As seguintes operações GET suportam mensagens do sistema:

- OBTER /teams/{team-id}/channels/{channel-id}/messages
- OBTER /teams/{team-td}/channels/{channel-id}/messages/{message-id}
- GET /chats/{chat-id}/messages
- GET /chats/{chat-id}/messages/{message-id}

Para obter detalhes, consulte [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-v1.0&preserve-view=true).

## <a name="supported-change-notifications"></a>Suporta alteração de notificações

As seguintes alterações de notificações suportam mensagens do sistema:

- Assinar para mensagens em um canal - /teams/{team-id}/channels/{channel-id}/messages
- Assinar para mensagens em um chat - /chats/{chat-id}/messages

Para obter detalhes, consulte [Alterar notificações para mensagens](teams-changenotifications-chatmessage.md).


## <a name="supported-system-message-events"></a>Suporta eventos de mensagem do sistema

| Evento   |  Tipo de mensagem do sistema   | Aplicável a |
|:--------|:--------------|:--------------|
| Encerramento da chamada | [callEndedEventMessageDetail](#call-ended) | Chat, Canal |
| Gravação da chamada | [callRecordingEventMessageDetail](#call-recording) | Chat, Canal |
| Inicio da chamada | [callStartedEventMessageDetail](#call-started) | Chat, Canal |
| Transcrição da chamada | [callTranscriptEventMessageDetail](#call-transcript) | Chat, Canal |
| Canal adicionado | [channelAddedEventMessageDetail](#channel-added) | Equipe |
| Canal excluído | [channelDeletedEventMessageDetail](#channel-deleted) | Equipe |
| Descrição atualizada do canal | [channelDescriptionUpdatedEventMessageDetail](#channel-description-updated) | Canal |
| Canal renomeado | [channelRenamedEventMessageDetail](#channel-renamed) | Canal |
| Canal definido como favorito | [channelSetAsFavoriteByDefaultEventMessageDetail](#channel-set-as-favorite-by-default) | Canal |
| Canal removido da definição como favorito | [channelUnsetAsFavoriteByDefaultEventMessageDetail](#channel-unset-as-favorite-by-default) | Canal |
| Chat renomeado | [chatRenamedEventMessageDetail](#chat-renamed) | Chat |
| Atualização da função de membro da conversa | [conversationMemberRoleUpdatedEventMessageDetail](#conversation-member-role-updated) | Canal, Equipe |
| Política de reuniões atualizada | [meetingPolicyUpdatedEventMessageDetail](#meeting-policy-updated) | Chat |
| Membros adicionados | [membersAddedEventMessageDetail](#members-added) | Chat, Canal, Equipe |
| Membros excluídos | [membersDeletedEventMessageDetail](#members-deleted) | Chat, Canal, Equipe |
| Membros que ingressaram | [membersJoinedEventMessageDetail](#members-joined) | Chat |
| Membros que saíram | [membersLeftEventMessageDetail](#members-left) | Chat |
| Mensagem fixada | [messagePinnedEventMessageDetail](#message-pinned) | Chat |
| Mensagem desafixada | [messageUnpinnedEventMessageDetail](#message-unpinned) | Chat |
| Guia atualizada | [tabUpdatedEventMessageDetail](#tab-updated) | Chat, Canal |
| Equipe arquivada | [teamArchivedEventMessageDetail](#team-archived) | Equipe |
| Equipe criada | [teamCreatedEventMessageDetail](#team-created) | Equipe |
| Descrição atualizada da equipe | [teamDescriptionUpdatedEventMessageDetail](#team-description-updated) | Equipe |
| O ingresso em equipe foi desabilitado | [teamJoiningDisabledEventMessageDetail](#team-joining-disabled) | Equipe |
| O ingresso em equipe foi habilitado | [teamJoiningEnabledEventMessageDetail](#team-joining-enabled) | Equipe |
| Equipe renomeada | [teamRenamedEventMessageDetail](#team-renamed) | Equipe |
| Aplicativo do Teams instalado | [teamsAppInstalledEventMessageDetail](#teams-app-installed) | Chat, Canal, Equipe |
| Aplicativo do Teams removido | [teamsAppRemovedEventMessageDetail](#teams-app-removed) | Chat, Canal, Equipe |
| Aplicativo do Teams atualizado | [teamsAppUpgradedEventMessageDetail](#teams-app-upgraded) | Chat, Canal, Equipe |
| Equipe desarquivada | [teamUnarchivedEventMessageDetail](#team-unarchived) | Equipe |


> **Observação:** As mensagens do sistema aplicáveis a uma equipe são postadas no canal principal.


## <a name="json-response-examples"></a>Exemplos de resposta JSON

Os exemplos de JSON a seguir mostram as respostas para cada tipo de evento suportado.

### <a name="call-ended"></a>Encerramento da chamada

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callEndedEventMessageDetail",
    "callId": "9c848c0e-f906-4dfc-b22e-c68a785a587c",
    "callDuration": "PT59S",
    "callEventType": "meeting",
    "callParticipants": [{
      "participant": {
        "application": null,
        "device": null,
        "user": {
          "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
          "displayName": "Adele Vance ",
          "userIdentityType": "aadUser"
        }
      }
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-recording"></a>Gravação da chamada

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callRecordingEventMessageDetail",
    "callId": "c86c6052-410b-4e7c-b843-9a09f576e4d5",
    "callRecordingDisplayName": "Meeting Recording.mp4",
    "callRecordingUrl": "https://testtenant.sharepoint.com/sites/TestTeam/Shared%20Documents/General/Recordings/Meeting%20Recording.mp4?web=1",
    "callRecordingDuration": "PT40M19.26S",
    "callRecordingStatus": "success",
    "meetingOrganizer": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    },
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-started"></a>Inicio da chamada

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callStartedEventMessageDetail",
    "callId": "9c848c0e-f906-4dfc-b22e-c68a785a587c",
    "callEventType": "call",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-transcript"></a>Transcrição da chamada

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callTranscriptEventMessageDetail",
    "callId": "5b927778-760b-429e-8c4e-65b1802dd6c9",
    "callTranscriptICalUid": "040000008200E00074C5B7101A82E00800000000002C743F89CDD601000000000000000010000000CA87F90D9372ED45A399B5D75E854EE9 ",
    "meetingOrganizer": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-added"></a>Canal adicionado

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelAddedEventMessageDetail",
    "channelId": "19:e84f079882f44fa8bebb7343b9e8921a@thread.tacv2",
    "channelDisplayName": "Standard channel",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-deleted"></a>Canal excluído

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelDeletedEventMessageDetail",
    "channelId": "19:914b8c83915548c0bff588e510a6cf01@thread.tacv2",
    "channelDisplayName": "Standard channel",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-description-updated"></a>Descrição atualizada do canal

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "channelDescription": "Channel description updated",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-renamed"></a>Canal renomeado

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "channelDisplayName": "Standard channel rename",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-set-as-favorite-by-default"></a>Canal definido como favorito por padrão

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-unset-as-favorite-by-default"></a>Canal removido da definição como favorito por padrão

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="chat-renamed"></a>Chat renomeado

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.chatRenamedEventMessageDetail",
    "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
    "chatDisplayName": "Microsoft Teams Members",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="conversation-member-role-updated"></a>Atualização da função de membro da conversa

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
    "conversationMemberRoles": [
      "Owner"
    ],
    "conversationMemberUser": {
      "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
      "displayName": null,
      "userIdentityType": "aadUser"
    },
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="meeting-policy-updated"></a>Política de reuniões atualizada

```json
{
  "id": "1620732126822",
  "replyToId": null,
  "etag": "1620732126822",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-11T11:22:06.822Z",
  "lastModifiedDateTime": "2021-05-11T11:22:06.822Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
    "meetingChatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
    "meetingChatEnabled": true,
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-added"></a>Membros adicionados

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersAddedEventMessageDetail",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
    "members": [{
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      },
      {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    ],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-deleted"></a>Membros excluídos

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersDeletedEventMessageDetail",
    "members": [{
      "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
      "displayName": null,
      "userIdentityType": "aadUser"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-joined"></a>Membros que ingressaram

```json
{
  "id": "1620050140712",
  "replyToId": null,
  "etag": "1620050140712",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T13:55:40.712Z",
  "lastModifiedDateTime": "2021-05-03T13:55:40.712Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersJoinedEventMessageDetail",
    "members": [{
      "id": "2c3f5f34-ac9f-42e7-8b35-442ccac166cb",
      "displayName": "Alex (Guest)",
      "userIdentityType": "aadUser"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-left"></a>Membros que saíram

```json
{
  "id": "1620049976741",
  "replyToId": null,
  "etag": "1620049976741",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T13:52:56.741Z",
  "lastModifiedDateTime": "2021-05-03T13:52:56.741Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersLeftEventMessageDetail",
    "members": [{
      "id": "ee8af8acd3184068a935a1f207865620",
      "displayName": "Alex (Guest)",
      "userIdentityType": "anonymousGuest"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="message-pinned"></a>Mensagem fixada

```json
{
  "id": "1613453493532",
  "replyToId": null,
  "etag": "1613453493532",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-02-16T05:31:33.532Z",
  "lastModifiedDateTime": "2021-02-16T05:31:33.532Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:0ae61fd5f7f44791baddce0988e71bf3@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
"eventDetail": {
    "@odata.type": "#microsoft.graph.messagePinnedEventMessageDetail",
    "eventDateTime": "2022-05-02T20:11:08.335Z",
    "initiator": {
        "application": null,
        "device": null,
        "user": {
            "id": "28c10244-4bad-4fda-993c-f332faef94f0",
            "displayName": null,
            "userIdentityType": "aadUser"
        }
    }
  }
}
```

### <a name="message-unpinned"></a>Mensagem desafixada

```json
{  
  "replyToId": null,
  "etag": "1613453493532",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-02-16T05:31:33.532Z",
  "lastModifiedDateTime": "2021-02-16T05:31:33.532Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:0ae61fd5f7f44791baddce0988e71bf3@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
"eventDetail": {
    "@odata.type": "#microsoft.graph.messageUnpinnedEventMessageDetail",
    "eventDateTime": "2022-05-02T20:11:08.335Z",
    "initiator": {
        "application": null,
        "device": null,
        "user": {
            "id": "28c10244-4bad-4fda-993c-f332faef94f0",
            "displayName": null,
            "userIdentityType": "aadUser"
        }
    }
  }
}
```

### <a name="tab-updated"></a>Guia atualizada

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.tabUpdatedEventMessageDetail",
    "tabId": "tab::e82fa916-3c9a-407e-806b-0b9d8d7492c0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-archived"></a>Equipe arquivada

```json
{
  "id": "1623677858199",
  "replyToId": null,
  "etag": "1623677858199",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:37:38.199Z",
  "lastModifiedDateTime": "2021-06-14T13:37:38.199Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623677858199?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623677858199&parentMessageId=1623677858199",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamArchivedEventMessageDetail",
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-created"></a>Equipe criada

```json
{
  "id": "1623677858199",
  "replyToId": null,
  "etag": "1623677858199",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:37:38.199Z",
  "lastModifiedDateTime": "2021-06-14T13:37:38.199Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623677858199?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623677858199&parentMessageId=1623677858199",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamCreatedEventMessageDetail",
    "teamId": "19:715b7c2ea0894fe3a503f8958df1ef06@thread.tacv2",
    "teamDisplayName": "Test Team",
    "teamDescription": "This is a test team.",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-description-updated"></a>Descrição atualizada da equipe

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "teamDescription": "Team description updated",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-joining-disabled"></a>O ingresso em equipe foi desabilitado

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamJoiningDisabledEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-joining-enabled"></a>O ingresso em equipe foi habilitado

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamJoiningEnabledEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-renamed"></a>Equipe renomeada

```json
{
  "id": "1618821548765",
  "replyToId": null,
  "etag": "1618821548765",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-19T08:39:08.765Z",
  "lastModifiedDateTime": "2021-04-19T08:39:08.765Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618821548765?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618821548765&parentMessageId=1618821548765",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamRenamedEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "teamDisplayName": "Team rename",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-installed"></a>Aplicativo do Teams instalado

```json
{
  "id": "1620046494994",
  "replyToId": null,
  "etag": "1620046494994",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:54:54.994Z",
  "lastModifiedDateTime": "2021-05-03T12:54:54.994Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046494994?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046494994&parentMessageId=1620046494994",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppInstalledEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-removed"></a>Aplicativo do Teams removido

```json
{
  "id": "1620046597520",
  "replyToId": null,
  "etag": "1620046597520",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:56:37.52Z",
  "lastModifiedDateTime": "2021-05-03T12:56:37.52Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046597520?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046597520&parentMessageId=1620046597520",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppRemovedEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-upgraded"></a>Aplicativo do Teams atualizado

```json
{
  "id": "1620046597520",
  "replyToId": null,
  "etag": "1620046597520",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:56:37.52Z",
  "lastModifiedDateTime": "2021-05-03T12:56:37.52Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046597520?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046597520&parentMessageId=1620046597520",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppUpgradedEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-unarchived"></a>Equipe desarquivada

```json
{
  "id": "1623678060910",
  "replyToId": null,
  "etag": "1623678060910",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:41:00.91Z",
  "lastModifiedDateTime": "2021-06-14T13:41:00.91Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623678060910?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623678060910&parentMessageId=1623678060910",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamUnarchivedEventMessageDetail",
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```
