---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto claimsMappingPolicy foi aplicado.
ms.localizationpriority: medium
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 60e56f82302845dbb4d9aad6f6384be56c1dfa60
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59016691"
---
# <a name="list-appliesto"></a>Lista appliesTo

Namespace: microsoft.graph

Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual um [objeto claimsMappingPolicy](../resources/claimsmappingpolicy.md) foi aplicado. As declaraçõesMappingPolicy só podem ser aplicadas aos recursos [application](../resources/application.md) e [servicePrincipal.](../resources/serviceprincipal.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos `$expand` parâmetros de consulta , `$select` e `$top` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters). Ao `$expand` usar, certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}/appliesTo
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-1-java-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
        {
            "@odata.type": "#microsoft.graph.servicePrincipal",
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/335601aa-9c79-48a3-a9f7-d2a6ac9cb730/Microsoft.DirectoryServices.ServicePrincipal",
            "id": "335601aa-9c79-48a3-a9f7-d2a6ac9cb730",
            "accountEnabled": true,
            "createdDateTime": "2021-08-12T07:28:18Z",
            "appDisplayName": "My App",
            "appId": "e4d924fc-d18d-4e69-9a17-7095f311bf17",
            "appOwnerOrganizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "displayName": "My App",
            "publisherName": "Contoso",
            "servicePrincipalNames": [
                "e4d924fc-d18d-4e69-9a17-7095f311bf17"
            ],
            "servicePrincipalType": "Application",
            "signInAudience": "AzureADMyOrg"
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
