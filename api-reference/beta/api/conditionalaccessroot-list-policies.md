---
title: Listar políticas
description: Recupere uma lista de objetos conditionalAccessPolicy.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c1d56cde38b7dfd3acbff3c20d399c5b762f3da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382286"
---
# <a name="list-policies"></a><span data-ttu-id="49698-103">Listar políticas</span><span class="sxs-lookup"><span data-stu-id="49698-103">List policies</span></span>

<span data-ttu-id="49698-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49698-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49698-105">Recupere uma lista de objetos [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="49698-105">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="49698-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="49698-106">Permissions</span></span>

<span data-ttu-id="49698-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49698-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49698-109">Permission type</span></span>                        | <span data-ttu-id="49698-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49698-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="49698-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49698-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49698-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="49698-112">Policy.Read.All</span></span> |
|<span data-ttu-id="49698-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49698-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49698-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49698-114">Not supported.</span></span> |
|<span data-ttu-id="49698-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49698-115">Application</span></span>                            | <span data-ttu-id="49698-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="49698-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49698-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49698-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49698-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="49698-118">Optional query parameters</span></span>

<span data-ttu-id="49698-119">Este método oferece suporte `$skip`aos `$top`parâmetros `$count`de `$filter`consulta `$orderBy`do, `$select` ,,, e OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="49698-119">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="49698-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="49698-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="49698-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49698-121">Request headers</span></span>

| <span data-ttu-id="49698-122">Nome</span><span class="sxs-lookup"><span data-stu-id="49698-122">Name</span></span>      |<span data-ttu-id="49698-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="49698-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49698-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="49698-124">Authorization</span></span> | <span data-ttu-id="49698-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="49698-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="49698-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49698-126">Request body</span></span>

<span data-ttu-id="49698-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="49698-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49698-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="49698-128">Response</span></span>

<span data-ttu-id="49698-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49698-129">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49698-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="49698-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49698-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49698-131">Request</span></span>

<span data-ttu-id="49698-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="49698-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49698-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="49698-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="c"></a>[<span data-ttu-id="49698-134">C#</span><span class="sxs-lookup"><span data-stu-id="49698-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49698-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49698-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49698-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49698-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49698-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="49698-137">Response</span></span>

<span data-ttu-id="49698-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="49698-138">The following is an example of the response.</span></span>

> <span data-ttu-id="49698-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49698-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
