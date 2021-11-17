---
title: Instalar o aplicativo para o usuário
description: Instale um aplicativo no escopo pessoal do usuário especificado.
author: akjo
doc_type: apiPageType
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: cb900a40dedcc8fad4e12fbf6ce12af39fa5e015
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031356"
---
# <a name="install-app-for-user"></a>Instalar o aplicativo para o usuário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Instale um [aplicativo](../resources/teamsapp.md) no escopo pessoal do usuário [especificado.](../resources/user.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{user-id | user-principal-name}/teamwork/installedApps
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação deve conter a ID do aplicativo de catálogo existente a ser adicionado.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|teamsApp|Cadeia de caracteres|A ID do aplicativo a ser acrescentado.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `201 Created`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->
```http
POST https://graph.microsoft.com/beta/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-add-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-add-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-add-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-add-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-add-teamsapp-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


