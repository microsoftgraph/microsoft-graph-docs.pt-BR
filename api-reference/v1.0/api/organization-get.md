---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
ms.localizationpriority: high
author: KuiGithui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 575ad102e16eb00f628e093149fa5b10a2f40fa4
ms.sourcegitcommit: a11c874a7806fb5825752c8348e12079d23323e4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2022
ms.locfileid: "65293998"
---
# <a name="get-organization"></a>Obter organização

Namespace: microsoft.graph

Obtenha as propriedades e relações da organização autenticada no momento.

Como o recurso da **organização** tem suporte para [extensões](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **organização**.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All |

> **Observação**: Os aplicativos que tem a permissão User.Read só conseguem ler as propriedades **id**, **displayName** e **verifiedDomains** da organização.  Todas as outras propriedades retornarão valores `null`. Para ler todas as propriedades, use Organization.Read.All.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de um objeto de [organização](../resources/organization.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/84841066-274d-4ec0-a5c1-276be684bdd3
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-organization-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-organization-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization/$entity",
    "id": "84841066-274d-4ec0-a5c1-276be684bdd3",
    "deletedDateTime": null,
    "businessPhones": [
        "425-555-0100"
    ],
    "city": null,
    "country": null,
    "countryLetterCode": "NL",
    "createdDateTime": "2021-08-02T10:30:06Z",
    "displayName": "Contoso",
    "isMultipleDataLocationsForServicesEnabled": null,
    "marketingNotificationEmails": [],
    "onPremisesLastSyncDateTime": null,
    "onPremisesSyncEnabled": null,
    "postalCode": null,
    "preferredLanguage": "en",
    "securityComplianceNotificationMails": [],
    "securityComplianceNotificationPhones": [],
    "state": null,
    "street": null,
    "technicalNotificationMails": [
        "admin@contoso.com"
    ],
    "tenantType": "AAD",
    "directorySizeQuota": {
        "used": 698,
        "total": 50000
    },
    "assignedPlans": [
        {
            "assignedDateTime": "2022-04-03T02:46:42Z",
            "capabilityStatus": "Deleted",
            "service": "Adallom",
            "servicePlanId": "932ad362-64a8-4783-9106-97849a1a30b9"
        },
        {
            "assignedDateTime": "2022-04-03T02:46:42Z",
            "capabilityStatus": "Deleted",
            "service": "MultiFactorService",
            "servicePlanId": "8a256a2b-b617-496d-b51b-e76466e88db0"
        },
        {
            "assignedDateTime": "2021-08-02T10:36:57Z",
            "capabilityStatus": "Enabled",
            "service": "exchange",
            "servicePlanId": "113feb6c-3fe4-4440-bddc-54d774bf0318"
        },
        {
            "assignedDateTime": "2021-08-02T10:36:02Z",
            "capabilityStatus": "Deleted",
            "service": "SCO",
            "servicePlanId": "882e1d05-acd1-4ccb-8708-6ee03664b117"
        }
    ],
    "privacyProfile": {
        "contactEmail": "",
        "statementUrl": ""
    },
    "provisionedPlans": [
        {
            "capabilityStatus": "Deleted",
            "provisioningStatus": "Success",
            "service": "Adallom"
        },
        {
            "capabilityStatus": "Enabled",
            "provisioningStatus": "Success",
            "service": "exchange"
        }
    ],
    "verifiedDomains": [
        {
            "capabilities": "Email, OfficeCommunicationsOnline",
            "isDefault": true,
            "isInitial": true,
            "name": "Contoso.com",
            "type": "Managed"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
