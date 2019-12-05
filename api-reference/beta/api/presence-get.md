---
title: Obter presença
description: Obtenha as informações de presença de um usuário.
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 3d1b56dc8266eea42c773596c8e78e9e0ece5b6b
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844180"
---
# <a name="get-presence"></a>Obter presença

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as informações de [presença](../resources/presence.md) de um usuário.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é necessária para chamar essas APIs. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                  |
| :-------------- | :----------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Presence. Read, Presence. Read. All                         |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                         |
| Application                            | Sem suporte.                                  |

## <a name="http-requests"></a>Solicitações HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |


## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Presence](../resources/presence.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-your-own-presence-information"></a>Exemplo 1: obter suas próprias informações de presença

O exemplo a seguir mostra como obter suas próprias informações de presença. Esta operação requer a permissão Presence. Read.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a>Exemplo 2: obter as informações de presença de outro usuário

O exemplo a seguir mostra como obter as informações de presença de outro usuário. Esta operação requer a permissão Presence. Read. All.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```http
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
