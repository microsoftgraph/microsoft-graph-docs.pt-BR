---
title: Obter conditionalAccessPolicy
description: Recupere as propriedades e as relações de um objeto conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d63de5409730b413d5f65e4e704b89b4681715d2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047242"
---
# <a name="get-conditionalaccesspolicy"></a><span data-ttu-id="bd15f-103">Obter conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="bd15f-103">Get conditionalAccessPolicy</span></span>

<span data-ttu-id="bd15f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd15f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd15f-105">Recupere as propriedades e as relações de [um objeto conditionalAccessPolicy.](../resources/conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bd15f-105">Retrieve the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd15f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd15f-106">Permissions</span></span>

<span data-ttu-id="bd15f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd15f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd15f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd15f-109">Permission type</span></span>                        | <span data-ttu-id="bd15f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd15f-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="bd15f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd15f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd15f-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd15f-112">Policy.Read.All</span></span> |
|<span data-ttu-id="bd15f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd15f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd15f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd15f-114">Not supported.</span></span> |
|<span data-ttu-id="bd15f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd15f-115">Application</span></span>                            | <span data-ttu-id="bd15f-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd15f-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd15f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd15f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd15f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd15f-118">Optional query parameters</span></span>

<span data-ttu-id="bd15f-119">Este método dá suporte ao `$select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd15f-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="bd15f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bd15f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd15f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd15f-121">Request headers</span></span>

| <span data-ttu-id="bd15f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bd15f-122">Name</span></span>      |<span data-ttu-id="bd15f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd15f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd15f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd15f-124">Authorization</span></span> | <span data-ttu-id="bd15f-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="bd15f-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd15f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd15f-126">Request body</span></span>

<span data-ttu-id="bd15f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd15f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd15f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd15f-128">Response</span></span>

<span data-ttu-id="bd15f-129">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd15f-129">If successful, this method returns a `200 OK` response code and the requested [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd15f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd15f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd15f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd15f-131">Request</span></span>

<span data-ttu-id="bd15f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd15f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd15f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd15f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="bd15f-134">C#</span><span class="sxs-lookup"><span data-stu-id="bd15f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd15f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd15f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd15f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd15f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd15f-137">Java</span><span class="sxs-lookup"><span data-stu-id="bd15f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conditionalaccesspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd15f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd15f-138">Response</span></span>

<span data-ttu-id="bd15f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd15f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="bd15f-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bd15f-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
            "mobileAppsAndDesktopClients",
            "exchangeActiveSync",
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
        "deviceStates": null,
        "devices": {
            "includeDevices": [
                "All"
            ],
            "excludeDevices": [
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


