---
title: Obter conversationMember
description: Recuperar um membro de um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a2c539b7240060a6434f5ece01dc242ae948a5f4
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379264"
---
# <a name="get-conversationmember"></a>Obter conversationMember

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegado (conta corporativa ou de estudante)|Chat.Read, Chat.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo |Chat.Read.All, Chat.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
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

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
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