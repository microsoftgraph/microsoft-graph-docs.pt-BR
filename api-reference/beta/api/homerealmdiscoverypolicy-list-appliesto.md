---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto homeRealmDiscoveryPolicy foi aplicado.
ms.localizationpriority: medium
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b94a6501cc7c51947ec61da50afcf2e3b07df5e2
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262083"
---
# <a name="list-appliesto"></a>Lista appliesTo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual um [objeto homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) foi aplicado. O homeRealmDiscoveryPolicy só pode ser aplicado aos [recursos servicePrincipal](../resources/serviceprincipal.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos parâmetros `$select` `$top` de consulta E OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta. Ele retornará um `404 Not Found` código de resposta se a política não tiver sido aplicada a nenhum objeto de diretório.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/6c6f154f-cb39-4ff9-bf5b-62d5ad585cde/appliesTo
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
        {
            "@odata.type": "#microsoft.graph.servicePrincipal",
            "id": "19c308f2-e088-464d-8ccb-7137b7bab660",
            "accountEnabled": true,
            "alternativeNames": [],
            "appDisplayName": "LinkedIn",
            "appId": "c8e5820f-8e41-4b7c-8937-42777eb592a4",
            "appOwnerOrganizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "displayName": "LinkedIn",
            "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=linkedin|ISV9.3|primary|z",
            "servicePrincipalNames": [
                "c8e5820f-8e41-4b7c-8937-42777eb592a4",
                "http://LinkedIn/1a2d95c1-3cc7-46ad-82dd-2c768ae1b4ff"
            ],
            "servicePrincipalType": "Application",
            "signInAudience": "AzureADMyOrg",
            "tags": [
                "4d57f64e-9941-4df2-bb70-8d9a2a38ab91",
                "WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1",
                "WindowsAzureActiveDirectoryIntegratedApp"
            ],
            "appRoles": [
                {
                    "allowedMemberTypes": [
                        "User"
                    ],
                    "description": "msiam_access",
                    "displayName": "msiam_access",
                    "id": "01c2bb8e-0895-42c8-b950-3ec8abc7a012",
                    "isEnabled": true,
                    "origin": "Application",
                    "value": null
                }
            ],
            "keyCredentials": [],
            "oauth2PermissionScopes": [
                {
                    "adminConsentDescription": "Allow the application to access LinkedIn on behalf of the signed-in user.",
                    "adminConsentDisplayName": "Access LinkedIn",
                    "id": "6edde65d-3f90-4251-9df2-0329b678b368",
                    "isEnabled": true,
                    "type": "User",
                    "userConsentDescription": "Allow the application to access LinkedIn on your behalf.",
                    "userConsentDisplayName": "Access LinkedIn",
                    "value": "user_impersonation"
                }
            ],
            "passwordCredentials": []
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

