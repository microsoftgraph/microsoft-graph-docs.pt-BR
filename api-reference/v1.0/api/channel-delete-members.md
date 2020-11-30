---
title: Remover membro do canal
description: Remover um membro de um canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e0f9d8a17403b1d4d7833abcc3f3bdcb69bee741
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387812"
---
# <a name="remove-member-from-channel"></a>Remover membro do canal

Namespace: microsoft.graph
 
Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md). Essa operação só é permitida para canais com um valor de **membershiptype** de `private` .


## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegado (conta corporativa ou de estudante)| ChannelMember.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application| ChannelMember.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored"} -->

```http
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "delete_channel-member"
} -->
```http
DELETE https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

- [Remover membro da equipe](team-delete-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete_channel_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
