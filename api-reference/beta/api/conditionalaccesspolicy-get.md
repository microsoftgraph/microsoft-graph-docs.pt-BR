---
title: Obter conditionalAccessPolicy
description: Recupere as propriedades e os relacionamentos de um objeto conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3d3d0f4a33eb8a6386d3b479a17233534f61da12
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747571"
---
# <a name="get-conditionalaccesspolicy"></a><span data-ttu-id="9cf47-103">Obter conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="9cf47-103">Get conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf47-104">Recupere as propriedades e os relacionamentos de um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9cf47-104">Retrieve the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cf47-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cf47-105">Permissions</span></span>

<span data-ttu-id="9cf47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cf47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf47-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cf47-108">Permission type</span></span>                        | <span data-ttu-id="9cf47-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cf47-109">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="9cf47-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cf47-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cf47-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cf47-111">Policy.Read.All</span></span> |
|<span data-ttu-id="9cf47-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cf47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cf47-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cf47-113">Not supported.</span></span> |
|<span data-ttu-id="9cf47-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cf47-114">Application</span></span>                            | <span data-ttu-id="9cf47-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cf47-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cf47-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf47-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/policies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9cf47-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9cf47-117">Optional query parameters</span></span>

<span data-ttu-id="9cf47-118">Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9cf47-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9cf47-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9cf47-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cf47-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf47-120">Request headers</span></span>

| <span data-ttu-id="9cf47-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9cf47-121">Name</span></span>      |<span data-ttu-id="9cf47-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf47-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9cf47-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cf47-123">Authorization</span></span> | <span data-ttu-id="9cf47-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9cf47-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cf47-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf47-125">Request body</span></span>

<span data-ttu-id="9cf47-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cf47-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cf47-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf47-127">Response</span></span>

<span data-ttu-id="9cf47-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cf47-128">If successful, this method returns a `200 OK` response code and the requested [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cf47-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9cf47-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cf47-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cf47-130">Request</span></span>

<span data-ttu-id="9cf47-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cf47-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9cf47-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf47-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cf47-133">C#</span><span class="sxs-lookup"><span data-stu-id="9cf47-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cf47-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cf47-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cf47-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cf47-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9cf47-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cf47-136">Response</span></span>

<span data-ttu-id="9cf47-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cf47-137">The following is an example of the response.</span></span>

> <span data-ttu-id="9cf47-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cf47-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
    "id": "6b5e999b-0ba8-4186-a106-e0296c1c4358",
    "displayName": "Demo app for documentation",
    "createdDateTime": "2019-09-26T23:12:16.0792706Z",
    "modifiedDateTime": "2019-09-27T00:12:12.5986473Z",
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "medium",
            "low"
        ],
        "clientAppTypes": [
            "modern",
            "easSupported",
            "easUnsupported",
            "other"
        ],
        "applications": {
            "includeApplications": [
                "All"
            ],
            "excludeApplications": [
                "499b84ac-1321-427f-aa17-267ca6975798",
                "00000007-0000-0000-c000-000000000000",
                "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                "00000012-0000-0000-c000-000000000000",
                "797f4846-ba00-4fd7-ba43-dac1f8f63013",
                "05a65629-4c1b-48c1-a78b-804c4abdd4af",
                "7df0a125-d3be-4c96-aa54-591f83ff541c"
            ],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [
                "a702a13d-a437-4a07-8a7e-8c052de62dfd"
            ],
            "excludeUsers": [
                "124c5b6a-ffa5-483a-9b88-04c3fce5574a",
                "GuestsOrExternalUsers"
            ],
            "includeGroups": [],
            "excludeGroups": [],
            "includeRoles": [
                "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "cf1c38e5-3621-4004-a7cb-879624dced7c",
                "c4e39bd9-1100-46d3-8c65-fb160da0071f"
            ],
            "excludeRoles": [
                "b0f54661-2d74-4c50-afa3-1ec803f12efe"
            ]
        },
        "platforms": {
            "includePlatforms": [
                "all"
            ],
            "excludePlatforms": [
                "iOS",
                "windowsPhone"
            ]
        },
        "locations": {
            "includeLocations": [
                "AllTrusted"
            ],
            "excludeLocations": [
                "00000000-0000-0000-0000-000000000000",
                "d2136c9c-b049-47ae-b9cf-316e04ef7198"
            ]
        },
        "deviceStates": {
            "includeStates": [
                "All"
            ],
            "excludeStates": [
                "Compliant"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa",
            "compliantDevice",
            "domainJoinedDevice",
            "approvedApplication",
            "compliantApplication"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": [
            "ce580154-086a-40fd-91df-8a60abac81a0",
            "7f29d675-caff-43e1-8a53-1b8516ed2075"
        ]
    },
    "sessionControls": {
        "applicationEnforcedRestrictions": null,
        "persistentBrowser": null,
        "cloudAppSecurity": {
            "cloudAppSecurityType": "blockDownloads",
            "isEnabled": true
        },
        "signInFrequency": {
            "value": 4,
            "type": "hours",
            "isEnabled": true
        }
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
