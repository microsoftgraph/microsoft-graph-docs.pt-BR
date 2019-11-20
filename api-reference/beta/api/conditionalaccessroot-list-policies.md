---
title: Listar políticas
description: Recupere uma lista de objetos conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ed519aabb270648e83ae8dc3d9cf46cf8ff12e6
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747547"
---
# <a name="list-policies"></a><span data-ttu-id="60a23-103">Listar políticas</span><span class="sxs-lookup"><span data-stu-id="60a23-103">List policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a23-104">Recupere uma lista de objetos [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="60a23-104">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="60a23-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="60a23-105">Permissions</span></span>

<span data-ttu-id="60a23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60a23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a23-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60a23-108">Permission type</span></span>                        | <span data-ttu-id="60a23-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60a23-109">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="60a23-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60a23-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="60a23-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a23-111">Policy.Read.All</span></span> |
|<span data-ttu-id="60a23-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60a23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60a23-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60a23-113">Not supported.</span></span> |
|<span data-ttu-id="60a23-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60a23-114">Application</span></span>                            | <span data-ttu-id="60a23-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a23-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60a23-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60a23-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60a23-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60a23-117">Optional query parameters</span></span>

<span data-ttu-id="60a23-118">Este método oferece suporte `$skip`aos `$top`parâmetros `$count`de `$filter`consulta `$orderBy`do, `$select` ,,, e OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60a23-118">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="60a23-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="60a23-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60a23-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60a23-120">Request headers</span></span>

| <span data-ttu-id="60a23-121">Nome</span><span class="sxs-lookup"><span data-stu-id="60a23-121">Name</span></span>      |<span data-ttu-id="60a23-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="60a23-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60a23-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60a23-123">Authorization</span></span> | <span data-ttu-id="60a23-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="60a23-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="60a23-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60a23-125">Request body</span></span>

<span data-ttu-id="60a23-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60a23-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60a23-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a23-127">Response</span></span>

<span data-ttu-id="60a23-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60a23-128">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60a23-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60a23-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60a23-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60a23-130">Request</span></span>

<span data-ttu-id="60a23-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60a23-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60a23-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="60a23-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60a23-133">C#</span><span class="sxs-lookup"><span data-stu-id="60a23-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60a23-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60a23-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60a23-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60a23-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60a23-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="60a23-136">Response</span></span>

<span data-ttu-id="60a23-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60a23-137">The following is an example of the response.</span></span>

> <span data-ttu-id="60a23-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60a23-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies",
    "value": [
        {
            "id": "ad8d2b4a-8d30-413f-88b8-144c6c8d98d9",
            "displayName": "SimplePolicy1",
            "createdDateTime": null,
            "modifiedDateTime": null,
            "state": "disabled",
            "sessionControls": null,
            "conditions": {
                "signInRiskLevels": [],
                "clientAppTypes": [],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
                "applications": {
                    "includeApplications": [
                        "None"
                    ],
                    "excludeApplications": [],
                    "includeUserActions": []
                },
                "users": {
                    "includeUsers": [
                        "None"
                    ],
                    "excludeUsers": [],
                    "includeGroups": [],
                    "excludeGroups": [],
                    "includeRoles": [],
                    "excludeRoles": []
                }
            },
            "grantControls": {
                "operator": "OR",
                "builtInControls": [
                    "block"
                ],
                "customAuthenticationFactors": [],
                "termsOfUse": []
            }
        },
        {
            "id": "c558e346-969d-40a7-a64e-2df6c2c88490",
            "displayName": "SimplePolicy2",
            "createdDateTime": null,
            "modifiedDateTime": null,
            "state": "disabled",
            "sessionControls": null,
            "conditions": {
                "signInRiskLevels": [],
                "clientAppTypes": [],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
                "applications": {
                    "includeApplications": [
                        "None"
                    ],
                    "excludeApplications": [],
                    "includeUserActions": []
                },
                "users": {
                    "includeUsers": [
                        "None"
                    ],
                    "excludeUsers": [],
                    "includeGroups": [],
                    "excludeGroups": [],
                    "includeRoles": [],
                    "excludeRoles": []
                }
            },
            "grantControls": {
                "operator": "OR",
                "builtInControls": [
                    "mfa"
                ],
                "customAuthenticationFactors": [],
                "termsOfUse": []
            }
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List policies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
