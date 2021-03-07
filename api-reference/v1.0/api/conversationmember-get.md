---
title: Obter conversationMember
description: Obtenha um membro do bate-papo ou do canal.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 79c38e9f8f2dbe378198e01610c57453eb7a2ba8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515811"
---
# <a name="get-conversationmember"></a>Obter conversationMember

Namespace: microsoft.graph

Recuperar um [conversationMember](../resources/conversationmember.md) de um [chat](../resources/chatmessage.md) ou [canal](../resources/channel.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegada (conta corporativa ou de estudante)| Para recurso de **usuário** ou **chat**: Chat.ReadBasic, Chat.Read, Chat.ReadWrite<br/><br/>Para o recurso **canal**: ChannelMember.Read.All, ChannelMember.ReadWrite |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Para **usuário** ou **recurso de chat**: Não suportado.<br/><br/>Para o recurso **canal**: TeamMember.Read.Group*, ChannelMember.Read.All, ChannelMember.ReadWrite.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso](https://aka.ms/teams-rsc).

> [!NOTE]
> É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!--
{
  "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
