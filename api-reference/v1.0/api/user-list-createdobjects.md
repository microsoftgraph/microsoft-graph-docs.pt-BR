---
title: Listar createdObjects
description: Obtenha uma lista de objetos de diretório criados pelo usuário.
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c13c3d9f2e5a06c01baacfd1cc2227a4ea2e01ae
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016004"
---
# <a name="list-createdobjects"></a>Listar createdObjects

Namespace: microsoft.graph

Obtenha uma lista de objetos de diretório criados pelo usuário. Essa API retorna apenas os objetos de diretório que foram criados por um usuário que não está em nenhuma função de administrador; caso contrário, ele retorna um objeto vazio.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | User.Read, User.ReadWrite    |
|Aplicativo | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
GET /me/createdObjects
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-createdobjects-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Este é um exemplo de resposta. A partir da resposta, o usuário criou um grupo Microsoft 365, um aplicativo e sua entidade de serviço.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "92f3d47b-86cc-4b90-953e-8ec7f83ef45f",
      "displayName": "Contoso volunteer roster",
      "groupTypes": [
        "Unified"
      ],
      "mail": "volunteers@contoso.com",
      "mailEnabled": true,
      "mailNickname": "volunteers"
    },
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "5847962e-c746-4707-a657-f80b5b71f429",
      "appId": "254e989a-1b8c-4f8c-84e8-9dea78e9d283",
      "displayName": "ConVol",
      "publisherDomain": "contoso.com",
      "signInAudience": "AzureADMyOrg"
    },
    {
      "@odata.type": "#microsoft.graph.servicePrincipal",
      "id": "ea6a54da-62be-4cdc-9860-3ed68a43d8f6",
      "accountEnabled": true,
      "appDisplayName": "ConVol",
      "appDescription": null,
      "appId": "254e989a-1b8c-4f8c-84e8-9dea78e9d283",
      "displayName": "ConVol",
      "servicePrincipalNames": [
        "254e989a-1b8c-4f8c-84e8-9dea78e9d283"
      ],
      "servicePrincipalType": "Application",
      "signInAudience": "AzureADMyOrg",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
