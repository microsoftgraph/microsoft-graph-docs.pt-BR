---
title: Obter permissionGrantPolicy
description: Recupere um único objeto permissionGrantPolicy.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 3f03bca84fa82bd7b9763906696baa23ad2168ca
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112533"
---
# <a name="get-permissiongrantpolicy"></a>Obter permissionGrantPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere um único [objeto permissionGrantPolicy.](../resources/permissiongrantpolicy.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Neste exemplo, a política solicitada é a política interna de concessão de permissão , que inclui permissões delegadas classificadas como baixas, para aplicativos de editores verificados ou aplicativos registrados `microsoft-user-default-low` neste locatário.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permissiongrantpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies/microsoft-user-default-low
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-permissiongrantpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-permissiongrantpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. A política tem dois conjuntos de condições, um que corresponde à permissão delegada classificada para aplicativos cliente registrados nesse locatário e o outro que corresponde a permissões delegadas classificadas para aplicativos de editores verificados (independentemente de qual locatário o aplicativo está `includes` `low` `low` registrado).

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "microsoft-user-default-low",
    "displayName": "Default User Low Risk Policy",
    "description": "All low risk permissions are consentable by member type users by default.",
    "includes": [
        {
            "id": "cb0c20dd-919d-40c5-ba6d-7ffb233b4b0b",
            "permissionClassification": "low",
            "permissionType": "delegated",
            "resourceApplication": "any",
            "permissions": [ "all" ],
            "clientApplicationIds": [ "all" ],
            "clientApplicationTenantIds": [ "11e37ee2-48fe-42e0-aab9-07d0bb165353" ],
            "clientApplicationPublisherIds": [ "all" ],
            "clientApplicationsFromVerifiedPublisherOnly": false,
            "certifiedClientApplicationsOnly": false
        },
        {
            "id": "8ce99f96-730c-4ebd-8397-07ee65942b97",
            "permissionClassification": "low",
            "permissionType": "delegated",
            "resourceApplication": "any",
            "permissions": [ "all" ],
            "clientApplicationIds": [ "all" ],
            "clientApplicationTenantIds": [ "all" ],
            "clientApplicationPublisherIds": [ "all" ],
            "clientApplicationsFromVerifiedPublisherOnly": true,
            "certifiedClientApplicationsOnly": false
        }
    ],
    "excludes": []
}
```
