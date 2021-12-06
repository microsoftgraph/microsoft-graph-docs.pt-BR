---
title: Listar appManagementPolicies
description: Obter uma lista de políticas de gerenciamento de aplicativos.
ms.localizationpriority: medium
author: madansr7
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c1da2cf2e1289c1216f769eec0aa3858ec92ed61
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982697"
---
# <a name="list-appmanagementpolicies"></a>Listar appManagementPolicies

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos appManagementPolicy.](../resources/appManagementPolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                |
| :------------------------------------- | :--------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                             |
| Aplicativo                            | Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte `$select` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$top` a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/appManagementPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objeto appManagementPolicy](../resources/appManagementPolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_appManagementPolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/appManagementPolicies
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-appmanagementpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-appmanagementpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-appmanagementpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-appmanagementpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-appmanagementpolicies-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appManagementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/appManagementPolicies",
   "value": [
      {
         "id": "db9d4b58-3488-4da4-9994-49773c454e33",
         "displayName": "Custom app management policy",
         "description": "Custom policy that enforces app management restrictions on specific applications and service principals.",
         "isEnabled": false,
         "restrictions": {
            "passwordCredentials": [
               {
                  "restrictionType": "passwordAddition",
                  "maxLifetime": null,
                  "restrictForAppsCreatedAfterDateTime": "2019-10-19T10:37:00Z"
               },
               {
                  "restrictionType": "passwordLifetime",
                  "maxLifetime": "P4DT12H30M5S",
                  "restrictForAppsCreatedAfterDateTime": "2017-10-19T10:37:00Z"
               },
               {
                  "restrictionType": "symmetricKeyAddition",
                  "maxLifetime": null,
                  "restrictForAppsCreatedAfterDateTime": "2021-10-19T10:37:00Z"
               },
               {
                  "restrictionType": "symmetricKeyLifetime",
                  "maxLifetime": "P4D",
                  "restrictForAppsCreatedAfterDateTime": "2014-10-19T10:37:00Z"
               }
            ],
            "keyCredentials": [
               {
                  "restrictionType": "asymmetricKeyLifetime",
                  "maxLifetime": "P90D",
                  "restrictForAppsCreatedAfterDateTime": "2014-10-19T10:37:00Z"
               }
            ]
         }
      }
   ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "get appManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
