---
title: Obter calendarPermission
description: Obter as propriedades e as relações do objeto calendarpermission.
author: Harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6e2c39aba8068973476b95d6eb3f91732cb3e81e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012357"
---
# <a name="get-calendarpermission"></a>Obter calendarPermission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o objeto de permissões especificado de um usuário ou calendário de grupo que foi compartilhado.

## <a name="permissions"></a>Permissões

Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Calendário | Delegado (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Aplicativo |
|:-----|:-----|:-----|:-----|
| calendário do usuário | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite | Calendars.Read, Calendars.ReadWrite |
| calendário de grupo | Group.Read.All, Group.ReadWrite.All | Sem suporte. | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

Obter as permissões especificadas do calendário principal de um usuário:
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

Obter as permissões especificadas de um calendário de grupo:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

Obter as permissões especificadas do calendário do usuário que contém o evento identificado:
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [calendarPermission](../resources/calendarpermission.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-calendarpermission-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": false,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
