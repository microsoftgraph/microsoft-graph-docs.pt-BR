---
title: 'chat: markChatReadForUser'
description: Marque um chat como lido até a hora atual ou a última mensagem recebida ou enviada.
author: sweta-thapliyal
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d20031641befc87ef198544798adc397560b3982
ms.sourcegitcommit: f9e71d3b8a54a98c282ef49783babe5698300c06
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2021
ms.locfileid: "60793971"
---
# <a name="chat-markchatreadforuser"></a>chat: markChatReadForUser
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Marque um [chat](../resources/chat.md) como lido para um usuário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Chat.ReadWrite|
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chat-id}/markChatReadForUser
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|tenantId|String|ID de locatário do usuário.|
|usuário|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Usuário para o que ler o chat.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chat_markchatreadforuser"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/19:7d898072-792c-4006-bb10-5ca9f2590649_8ea0e38b-efb3-4757-924a-5f94061cf8c2@unq.gbl.spaces/markChatReadForUser
Content-Type: application/json
Content-length: 106

{
 "user": {
    "id" : "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
  },
  "tenantId": "2a690434-97d9-4eed-83a6-f5f13600199a"
}
```


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

