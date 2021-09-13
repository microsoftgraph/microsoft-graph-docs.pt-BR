---
title: Excluir conversationMember
description: Excluir conversationMember de um canal.
author: akjo
doc_type: apiPageType
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: 396eba04ab1029f550a7ec141f4b52449cdc8f13
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59050737"
---
# <a name="delete-conversationmember"></a>Excluir conversationMember

Namespace: microsoft.graph

Excluir uma [conversaMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegada (conta corporativa ou de estudante)| ChannelMember.ReadWrite.All |
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| ChannelMember.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
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

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[C#](#tab/csharp)

# <a name="javascript"></a>[JavaScript](#tab/javascript)

# <a name="objective-c"></a>[Objective-C](#tab/objc)

---

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
